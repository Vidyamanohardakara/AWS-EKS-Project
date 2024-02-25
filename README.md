# AWS-EKS-Project
Steps to create AWS EKS cluster
1) eksctl create cluster --name demo-cluster-1 --region ap-south-1 --fargate
2) aws eks update-kubeconfig --name demo-cluster-1 --region ap-south-1
3) Create fargate profile
   eksctl create fargateprofile --cluster demo-cluster-1 --region ap-south-1 --name alb-sample-app --namespace game-2048
