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
kubectl apply -f provisioner.yaml
kubectl apply -f nodetemplate.yaml
kubectl apply -f deployment.yaml


kubectl delete -f deployment.yaml
kubectl delete -f nodetemplate.yaml
kubectl delete -f provisioner.yaml
