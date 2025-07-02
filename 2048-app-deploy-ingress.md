2048 App
Create Fargate profile
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048
Deploy the deployment, service and Ingress
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml

![image](https://github.com/user-attachments/assets/8690108e-ff31-41c7-b06f-3b628c5e6ccb)

