# AWS Serverless Email Notification System

## Overview
This project implements an event-driven serverless architecture using AWS services.
Whenever a file is uploaded to an Amazon S3 bucket, an AWS Lambda function is triggered,
which sends an email notification using Amazon SNS.

## Architecture
S3 (File Upload) → Lambda (Trigger) → SNS (Email Notification)

## AWS Services Used
- Amazon S3 – Event source & storage
- AWS Lambda – Serverless compute
- Amazon SNS – Email notifications
- IAM – Secure access control

## Features
- Fully serverless architecture
- Event-driven and automated
- Secure IAM roles with least privilege
- Cost-optimized (AWS Free Tier)

## How It Works
1. User uploads a file to S3
2. S3 triggers Lambda via event notification
3. Lambda publishes a message to SNS
4. SNS sends an email to subscribed users

## Deployment Steps
1. Create S3 bucket
2. Create SNS topic and email subscription
3. Create IAM role for Lambda
4. Deploy Lambda function
5. Configure S3 event trigger

## Security Best Practices
- No hardcoded AWS credentials
- IAM least privilege
- No EC2 or server exposure

## Cost
This project runs under AWS Free Tier with zero cost.

## Author
Rohini Longadge
