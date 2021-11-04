# AWS get started

This repository describes step by step how to create a infrastructure on AWS

It is based on the [AWS tutorial from Hashicorp](https://learn.hashicorp.com/tutorials/terraform/infrastructure-as-code?in=terraform/aws-get-started)


# Prerequisites
Install terraform [See documentation](https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started)

Install AWS cli [See documentation](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

# How to

## create the infrastructure
1. Clone the repository to your local machine
```
git clone https://github.com/munnep/aws_get_started
```
2. Change your directory
```
cd aws_get_started
```
3. Terraform initialize
```
terraform init
```
5. Terraform plan
```
terraform plan
```
6. Terraform apply
```
terraform apply
```
7. Sample output
```
...
...
...
Plan: 1 to add, 0 to change, 0 to destroy.

Do you want to perform these actions?
  Terraform will perform the actions described above.
  Only 'yes' will be accepted to approve.

  Enter a value: yes

aws_instance.app_server: Creating...
aws_instance.app_server: Still creating... [10s elapsed]
aws_instance.app_server: Still creating... [20s elapsed]
aws_instance.app_server: Still creating... [30s elapsed]
```
8. Check your current state file with the following command to see the infrastructure terraform created. 
```
terraform show
```
9. To just list the resources use the following
```
terraform state list
```
10. destroy the infrastructure
```
terraform destroy
```