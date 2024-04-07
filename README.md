# AWS Cloud Native Web Application And Infrastructure as Code
This repository contains links to my python web application and AWS infrastructure code configurations. In this project I tried to separate my application , infrastructure code and lambda function code in separate respositories as per the best deployment practices and utilized the github actions to create and end to end deployment cycle for my application.
Below are the repository names and links to them -

## 1. Infrastructure - https://github.com/sagar-malhotra/infrastructure
The infrastructure repository contains the cloudformation template the is being used to provision all the AWS infrastructure elements needed for the python application deployment and security. Please visit the link for more information on the repository.

- AWS CloudFormation
  - Architect and provision AWS resources for the Web App.
  - Configures networking components, auto-scaling groups, and database services via RDS.
  - AWS  resources deployed - VPC, Internet Gateway, VPC Gateway Attachment, Public Route Table, Route for Public Route Table, Subnets (public and private) in multiple Availability Zones, Subnet Route Table Associations, Security Groups for EC2 instances and databases, Amazon S3 Bucket, Amazon RDS (Relational Database Service) instance, Amazon DynamoDB Table, IAM (Identity and Access Management) roles and policies for EC2 instances, Lambda functions, and SES (Simple Email Service),Lambda Function
SNS (Simple Notification Service) Topic, Auto Scaling Group, CloudWatch Alarms for scaling policies based on CPU utilization , Elastic Load Balancer (Application Load Balancer), Elastic Load Balancer Listener ,Elastic Load Balancer Target Group, Route 53 Record Set for Load Balancer Alias

- CI/CD Pipeline
  - GitHub Actions workflow to continuously integrate and deploy the application.
  - Automates Amazon Machine Image (AMI) creation upon each code commit.

## 2. WebApp - https://github.com/sagar-malhotra/webapp
The webapp repository cotains the python application code to be deployed along with the github action workflows. For more information on the webapp and deployment please visit the link attached above.

Functionality of Web Applications

- Effective Account Administration
  - Ensuring the security of user profiles through a stringent creation process and email validation.
  - Guaranteeing that only authorized users have access to essential features.

- Document Handling
  - Comprehensive management of documents throughout their lifecycle directly within the application.
  - Supported by AWS S3 for dependable and scalable storage options.

- Incorporated Email Alert Mechanism
  - Employing AWS SNS to activate AWS Lambda functions.
  - Simplifying the dispatch of verification emails via AWS SES.
  - Maintaining thorough records of email activities and tokens using DynamoDB.

## 3. Serverless - https://github.com/sagar-malhotra/serverless
The Serveless repository contains the lambda function code responsible for handling the user verfication process after sign up and the github action workflow responsible for deploying the lambda function. For more information please visit the repository from the link attached above.
