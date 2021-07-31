# Project Setup And Stack Deployment With S3 Bucket

## Class Notes: -

Working with AWS we are going to use serverless portion of it. It is made mush easier with CDK, AWS centralized every thing in the form of cloud formation and then CDK and provided minimalist constructs so we can call them for configuration. Cloud formation is web assembly but we are going to use typescript for working with CDK. All the resources can be written in high level programming language and are reusable. A CDK app is made up of multiple stacks and CDK use cloud formation so, our code is converted into that.

## Steps: -

- Signup to AWS

- Create IAM user

  - Navigate to IAM section of the services.
  - Select users from access management
  - Select user name and grant programmatic access
  - Add to a group or create new with permissions
  - Tags (optional)
  - Review and create user
  - At the end access key and id will be generated

- Install TypeScript

  - "npm install -g typescript"

- Install AWS CLI

  - Download and install from [here](https://awscli.amazonaws.com/AWSCLIV2.msi)
  - "aws --version"

- Install AWS SAM CLI

  - Create AWS account
  - Create IAM user
  - Install docker
    - [Downlaod](https://docs.docker.com/docker-for-windows/install/)
    - Configure shared drives
    - "docker ps"
  - Install CLI
    - [Downalod](https://github.com/aws/aws-sam-cli/releases/latest/download/AWS_SAM_CLI_64_PY3.msi)
    - "sam --version"
  - Install Git

- Install AWS CDK
  - "aws configure"
  - "npm install -g aws-cdk"
  - "cdk --version"

## Reading Material: -

- [What is AWS CDK?](https://serverless-stack.com/chapters/what-is-aws-cdk.html)
- [AWS CDK in TypeScript](https://docs.aws.amazon.com/cdk/latest/guide/work-with-cdk-typescript.html)
- [AWS CDK and Typescript: Deploy a static React app to S3](https://medium.com/swlh/aws-cdk-and-typescript-deploy-a-static-react-app-to-s3-df74193e9e3d)
- [Signup for a AWS Fee Tier](https://aws.amazon.com/free/)
- [Get and setup AWS Credentials](https://docs.aws.amazon.com/toolkit-for-vscode/latest/userguide/aws-credentials.html)
- [Create IAM User](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html)
- [Install TypeScript](https://www.npmjs.com/package/typescript)
- [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- [Installing the AWS SAM CLI - This is an AWS CLI tool that helps you develop, test, and analyze your serverless applications locally](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
- [Install AWS CDK](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)
- [Understand the key concepts](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)
