EKS Cluster Setup
-----------------

Uses terraform module https://github.com/terraform-aws-modules/terraform-aws-eks

To setup Kubernetes Cluster using EKS

```
tfenv install 0.12.0
tfenv use 0.12.0
aws-vault exec shibata -- terraform init
aws-vault exec shibata -- terraform plan -out=eks-1.tfplan
aws-vault exec shibata -- terraform apply eks-1.tfplan
```


