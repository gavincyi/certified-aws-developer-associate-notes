# Certified AWS Associate Developer Notes

### My notes in preparation for the 2020 AWS developer associate exam 

## Table of contents

- AWS Fundamentals
    - [IAM: Identity Access & Management](1-aws-fundamentals/iam.md)
    - [EC2: Virtual Machines](1-aws-fundamentals/ec2.md)
    - [Security Groups](1-aws-fundamentals/security-groups.md)
    - [ELB: Elastic Load Balancers](1-aws-fundamentals/elb.md)
    - [ASG: Auto Scaling Group](1-aws-fundamentals/asg.md)
    - [EBS Volumes](1-aws-fundamentals/ebs.md)
    - [RDS: Relational Database Service](1-aws-fundamentals/rds.md)
    - [Route 53](1-aws-fundamentals/route53.md)
    - [ElastiCache](1-aws-fundamentals/elasticache.md)
    - [VPC: Virtual Private Cloud](1-aws-fundamentals/vpc.md)
    - [S3 Buckets](1-aws-fundamentals/s3.md)

- AWS Deep Dive
    - [CLI: Command Line Interface](2-aws-deep-dive/cli.md)
    - [SDK: Software Development Kit](2-aws-deep-dive/sdk.md)
    - [Elastic Beanstalk](2-aws-deep-dive/elastic-beanstalk.md)
    - [CICD: Continuous Integration and Deployment](2-aws-deep-dive/cicd/cicd.md)
        - [CodeCommit](2-aws-deep-dive/cicd/codecommit.md)
        - [CodePipeline](2-aws-deep-dive/cicd/codepipeline.md)
        - [CodeBuild](2-aws-deep-dive/cicd/codebuild.md)
        - [CodeDeploy](2-aws-deep-dive/cicd/codedeploy.md)
    - [CloudFormation](2-aws-deep-dive/cloudformation/cloudformation.md)
    - [CloudWatch](2-aws-deep-dive/monitoring-and-audit/cloudwatch.md)
    - [Integration and Messaging](2-aws-deep-dive/integration-and-messaging/integration-and-messaging.md)
        - SQS
        - SNS
        - Kinesis

- [YAML](2-aws-deep-dive/yaml.md)

- [AWS Serverless](3-aws-serverless/serverless.md)
  - Lambda
  - DynamoDB
  - API Gateway
  - Cognito

- Docker based AWS services
  - ECS: Elastic Container Service
  - Elastic Container Registry
  - Fargate

- [Exam Preperation](#exam-preparation)


## Exam Preparation

- Exam details
    - Two question types:
        - Multiple Choice
        - Multiple response
    - Minimum passing score: 720/1000
    - Domains:
        - Deployment: CICD, Beanstalk, Serverless
        - Security: each service deep-dive + dedicated section
        - Development with AWS Services: Serverless, API, SDK, & CLI
        - Refactoring: Understand all the AWS services for the best migration
        - Monitoring and Troubleshooting: CloudWAtch, CloudTrail, X-Ray

    - Exam Guide:
        - [Certified Developer - Associate Exam PDF](https://d1.awsstatic.com/training-and-certification/docs-dev-associate/AWS_Certified_Developer_Associate-Exam_Guide_EN_1.4.pdf)

- EC2 + IAM Exam Checklist
  * Know how to SSH into EC2 (and change .pem file permissions) 
  * Know how to properly use security groups 
  * Know the fundamental differences between private vs public vs elastic IP 
  * Know how to use User Data to customize your instance at boot time 
  * Know that you can build custom AMI to enhance your OS 
  * EC2 instances are billed by the second and can be easily created and thrown away, welcome to the cloud!  
  Maybe on Exam:
  * Availability zones are in geographically isolated data centers
  * IAM users are NOT defined on a per-region basis
  * If you are getting a permission error exception when trying to SSH into your linux instance, then the key is missing chmod 400 permissions
  * If you are getting a network timeout when trying to SSH into your EC2 instance, then your security groups are misconfigured
  * Security groups reference IP address, CIDR block, Security group, but NOT DNS name
