# AWS EKS Guide

## Introduction
This guide provides a quick overview of setting up and managing an AWS Elastic Kubernetes Service (EKS) cluster, from initial setup to application deployment.

## Kubernetes Fundamentals
### EKS vs. Self-Managed Kubernetes
- **EKS Pros**: Managed control plane, automated updates, scalability, AWS integrations, secure and compliant, monitoring via CloudWatch.
- **EKS Cons**: Higher cost, less control over infrastructure.
- **Self-Managed Pros**: Cost-effective with EC2 options, full flexibility, experimental features.
- **Self-Managed Cons**: Complexity, maintenance overhead, scaling challenges.

## Setting Up AWS Environment for EKS
### Creating an AWS Account & IAM Users
1. **Create an AWS Account**: Sign up at [AWS](https://aws.amazon.com/).
2. **IAM Users**: Go to IAM > "Add user" > Set access types > Configure permissions > Enable MFA (optional).

### Configuring AWS CLI & kubectl
1. **AWS CLI**: Install via [AWS CLI Documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html) and configure using `aws configure`.
2. **kubectl**: Install via [kubectl Documentation](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

### Networking & Security Groups
1. **VPC & Subnets**: Create a VPC with public/private subnets.
2. **Security Groups**: Define inbound/outbound rules for worker nodes.
3. **Internet Gateway**: Attach an IGW to your VPC and update route tables for internet access.

