# High-Availability Web Application on AWS

This project demonstrates the setup of a high-availability web application on AWS using CloudFormation, Docker, and Kubernetes.

## Prerequisites
- AWS Account
- AWS CLI configured
- Docker installed
- Kubernetes cluster (EKS or Minikube)

## Setup Instructions

### 1. CloudFormation
Deploy the AWS infrastructure using CloudFormation templates.
```bash
aws cloudformation create-stack --stack-name myVpc --template-body file://cloudformation/vpc.yaml
aws cloudformation create-stack --stack-name myEC2 --template-body file://cloudformation/ec2.yaml
aws cloudformation create-stack --stack-name myRDS --template-body file://cloudformation/rds.yaml
aws cloudformation create-stack --stack-name myS3 --template-body file://cloudformation/s3.yaml
