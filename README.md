### Create AWS VPC Using Terraform
terraform init
terraform apply

### Create EKS Cluster
terraform apply

### Create Karpenter Controller IAM Role
terraform init
terraform apply

### Deploy Karpenter
terraform apply

### Deployment
kubectl apply -f k8s/provisioner.yaml
kubectl apply -f k8s/nodetemplate.yaml
kubectl apply -f k8s/deployment.yaml


kubectl delete -f k8s/deployment.yaml
kubectl delete -f k8s/nodetemplate.yaml
kubectl delete -f k8s/provisioner.yaml
