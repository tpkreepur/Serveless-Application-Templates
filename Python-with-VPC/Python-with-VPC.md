# Python-with-VPC

This template contains the AWS Role template and SAM template to create a Python function that has access to S3, VPC interfaces, Cloudtrail Logging, and Secrets Manager.

When using the SAM CLI to create the CloudFormation stack from this template, rember to tighten up the Role of the function to limit the scope of the resources to prevent any possible security issues.

All of the templates contain dummy information regarding the AWS Account ID. Please remove the dummy info in all the referenced ARNs and replace with your AWS information.

## [Python-with-VPC.yml](./Python-with-VPC.yml)

- The AWS Serverless Application Model template.

## [LambdaService-S3AccessReadOnlyRole.json](./LambdaService-S3AccessReadOnlyRole.json)

- Sample AWS IAM Role template to allow the proper permissions of the AWS services.

This template allows access to all the services in the "Action" portion with no restrictions to specific resources. Keep that in mind when deploying this role to your AWS tenant.
