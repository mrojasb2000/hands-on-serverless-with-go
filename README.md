# hands-on-serverless-with-go
Hands-On Serverless Application with Go

## Basic config Amazon Web Service
* brew install awscli

* aws --version

* ~/.aws/credentials

-[default]
- aws_access_key_id = AKIAJYZMNSSSMS4EKH6Q
- aws_secret_access_key = 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
- region=eu-central-1

* aws lambda list-functions --profile default --region us-east-1

* aws lambda list-functions --profile default --region us-east-1 --output <table|json|text>

* aws lambda list-functions --profile default --region us-east-1 --query Function[].FunctionName

* aws lambda list-functions --profile default --region us-east-1 | jq '.Function[].FunctionName'

## Create Golang project - Hello World

* go mod init github.com/mrojasb2000/hands-on-serverless-with-go/helloworld