Commands to run:
Init:

terraform init -backend-config=bucket=adam-jozefowicz-panda-devops-core-19 or terraform init -reconfigure -backend-config=bucket=adam-jozefowicz-panda-devops-core-19
Check what will be done:

terraform plan or terraform plan -var bucket_name=adam-jozefowicz-panda-devops-core-19
Apply configuration:

terraform apply -auto-approve or terraform apply -auto-approve -var bucket_name=adam-jozefowicz-panda-devops-core-19
Check the loadbalancer readiness:

watch -n 1 curl -s alb-xxxxxxxxx.us-east-1.elb.amazonaws.com
Destroy environment:
terraform destroy -auto-approve or terraform destroy -auto-approve -var bucket_name=adam-jozefowicz-panda-devops-core-19
