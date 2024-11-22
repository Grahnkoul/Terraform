Commands to run:
Init:

terraform init -backend-config=bucket=<name>-<surname>-panda-devops-core-<n> or terraform init -reconfigure -backend-config=bucket=<name>-<surname>-panda-devops-core-<n>
Check what will be done:

terraform plan or terraform plan -var bucket_name=<name>-<surname>-panda-devops-core-<n>
Apply configuration:

terraform apply -auto-approve or terraform apply -auto-approve -var bucket_name=<name>-<surname>-panda-devops-core-<n>
Check the loadbalancer readiness:

watch -n 1 curl -s alb-xxxxxxxxx.us-east-1.elb.amazonaws.com
Destroy environment:
terraform destroy -auto-approve or terraform destroy -auto-approve -var bucket_name=<name>-<surname>-panda-devops-core-<n>