
*** Setup de ambiente cross-account:*** 
* DevOps - Repositório SharedLibrary
* DevTools - Repositório da App + KMS + Pipeline
* Dev - Conta que vai rodar o ambiente ECS de Dev

*** DevOps *** 
aws cloudformation deploy --stack-name SetupDevOps --template-file DevOps-Account/SetupDevOps.yaml --capabilities CAPABILITY_NAMED_IAM --profile itau-lab-devops

*** DevTools *** 
aws cloudformation deploy --stack-name SetupDevTools --template-file DevTools-Account/SetupDevTools.yaml --capabilities CAPABILITY_NAMED_IAM --profile itau-lab-devtools 
