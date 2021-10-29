# bootcamp2020c52 - Introduction to AWS CDK

## Project Setup And Stack Deployment With S3 Bucket

- Signup on AWS
- Create IAM user
- Install AWS CLI
- Install AWS SAM CLI
- Install AWS CDK
- Create CDK Hello app

## Class Notes: -

Working with AWS we are going to use serverless portion of it. It is made mush easier with CDK, AWS centralized every thing in the form of cloud formation and then CDK and provided minimalist constructs so we can call them for configuration. Cloud formation is web assembly but we are going to use typescript for working with CDK. All the resources can be written in high level programming language and are reusable. A CDK app is made up of multiple stacks and CDK use cloud formation so, our code is converted into that.

An AWS CDK app is an application that uses the AWS CDK to define AWS infrastructure. An app defines one or more stacks. Stacks (equivalent to AWS CloudFormation stacks) contain constructs (L1, L2 or L3), each of which defines one or more concrete AWS resources.

AWS CloudFormation-only or L1 constructs correspond directly to resource types defined by AWS CloudFormation. These constructs are automatically generated from the AWS CloudFormation specification, so when a new AWS service is launched, the AWS CDK supports it as soon as AWS CloudFormation does. AWS CloudFormation resources always have names that begin with Cfn. For example, in the Amazon S3 module, CfnBucket is the L1 module for an Amazon S3 bucket.

Curated or constructs are developed by AWS to address specific use cases and simplify infrastructure development. They encapsulate L1 modules. For example, in S3 module, Bucket is the L2 module for an S3 bucket. L2 modules may also define supporting resources needed by the primary resource. Some services have more than one L2 module in the Construct Library for organizational purposes.

Patterns or L3 declare multiple resources to create entire AWS architectures for particular use cases. All the plumbing is already hooked up, and configuration is boiled down to a few important parameters. In the AWS Construct Library, patterns are in separate modules from L1 and L2 constructs.

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

- Create Hello world App [Demo](https://docs.aws.amazon.com/cdk/latest/guide/hello_world.html)
  - "mkdir step00_hello_cdk"
  - "cd step00_hello_cdk"
  - "cdk init app --language typescript"
  - "cdk ls"
  - "npm install @aws-cdk/aws-s3"
  - "add s3 bucket in the stack"
  - "npm run build"
  - "cdk synth"
  - "cdk deploy"
  - deployed stack can be viewd at "https://console.aws.amazon.com/cloudformation/home"
  - deployed bucket can be viewd at "https://s3.console.aws.amazon.com/s3/home"
  - "cdk diff"
  - "cdk destroy"

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
- [Install Docker to test apps locally](https://docs.docker.com/get-docker/)
- [Install the Toolkit for VS Code](https://docs.aws.amazon.com/toolkit-for-vscode/latest/userguide/setup-toolkit.html)
- [Understand the key concepts](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)

## Video Lecture

- [YouTube English](https://www.youtube.com/watch?v=UpuVx8c0-lA&ab_channel=PanacloudServerlessSaaSTraining)
- [Facebook English](https://web.facebook.com/zeeshanhanif/videos/10225191381716499?_rdc=1&_rdr)
- [YouTube Urdu](https://www.youtube.com/watch?v=xWF-LCTnSy4&ab_channel=PanacloudServerlessSaaSTraininginUrdu)
- [Facebook Urdu](https://web.facebook.com/zeeshanhanif/videos/10225203759985948?_rdc=1&_rdr)
