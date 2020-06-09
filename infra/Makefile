up:
	terraform apply --auto-approve -var environment=${ENV} 

down:
	terraform destroy --auto-approve -var environment=${ENV}

init:
	terraform init --backend-config="key=state/${ENV}.tfstate" --backend-config="dynamodb_table=RMIT-locktable-k1ers1" --backend-config="bucket=rmit-tfstate-k1ers1"
