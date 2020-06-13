up:
	terraform apply --auto-approve -var environment=${ENV} 

down:
	terraform destroy --auto-approve -var environment=${ENV}

init:
	terraform init --backend-config="key=state/${ENV}.tfstate" --backend-config="dynamodb_table=RMIT-locktable-l2ceda" --backend-config="bucket=rmit-tfstate-l2ceda"
