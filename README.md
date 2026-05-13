# Serverless Cloud Architecture Project

## Overview

This project demonstrates a secure serverless cloud-native application deployed on Amazon Web Services (AWS) using modern cloud architecture and managed AWS services.

The environment was designed to strengthen hands-on experience with scalable cloud infrastructure, IAM-aware authentication workflows, operational monitoring and serverless deployment practices. The project uses an e-commerce scenario to simulate real-world cloud architecture patterns including secure authentication, API management, centralized logging, monitoring and cloud-native service integration.

The architecture follows AWS Well-Architected Framework principles across security, operational excellence, reliability and performance efficiency considerations.

---

## Objectives

* Design and deploy a secure serverless cloud architecture on AWS
* Implement authentication and role-based access controls
* Build scalable API-driven backend workflows using managed AWS services
* Integrate cloud monitoring, logging and operational visibility workflows
* Apply AWS Well-Architected Framework principles
* Strengthen hands-on experience with cloud-native deployment practices

---

## AWS Services Used

### Compute

* AWS Lambda

### Networking & API Management

* Amazon API Gateway
* Amazon CloudFront

### Storage

* Amazon S3

### Database

* Amazon DynamoDB

### Security & Identity

* Amazon Cognito
* AWS IAM
* AWS SSM Parameter Store

### Monitoring & Visibility

* Amazon CloudWatch
* AWS X-Ray

### Messaging & Notifications

* Amazon SNS

### Payment Integration

* Stripe Checkout (Sandbox Environment)

---

## Security & IAM Components

The project incorporated multiple cloud security and identity management concepts including:

* Amazon Cognito for user authentication and authorization
* Role-based access controls for guest, authenticated user and administrative workflows
* IAM least-privilege access configuration across AWS services
* Secure secret and configuration storage using AWS SSM Parameter Store
* HTTPS-only access enforcement through CloudFront and API Gateway
* CloudWatch logging and monitoring for operational visibility
* JWT-based authentication flows for protected API access

---

## Architecture Overview

The frontend application was hosted on Amazon S3 and distributed through Amazon CloudFront for secure and scalable global delivery.

Backend requests were routed through Amazon API Gateway to AWS Lambda functions responsible for application logic, authentication workflows and payment integration. DynamoDB was used as the primary database for storing products and order information.

Amazon Cognito handled authentication and user management while CloudWatch and X-Ray provided monitoring, logging and operational visibility across the environment.

---

## Application Workflow

1. User accesses the frontend application through CloudFront
2. Frontend interacts with API Gateway endpoints
3. API Gateway routes requests to Lambda functions
4. Lambda functions process business logic and interact with DynamoDB
5. Cognito manages authentication and authorization workflows
6. Stripe Checkout handles payment processing
7. SNS sends order confirmation notifications
8. CloudWatch and X-Ray provide monitoring and logging visibility

---

## Monitoring & Operational Visibility

Operational monitoring and visibility workflows were implemented using:

* Amazon CloudWatch logs and metrics
* AWS X-Ray distributed tracing
* API monitoring and logging
* Lambda execution monitoring
* Centralized operational visibility across serverless components

These monitoring capabilities supported troubleshooting, observability and application health tracking across the cloud environment.

---

## Skills Demonstrated

* AWS cloud architecture
* Serverless deployment practices
* IAM and authentication workflows
* Cloud-native application deployment
* API-driven backend integration
* Secure configuration management
* Cloud monitoring and operational visibility
* Logging and observability concepts
* Role-based access control implementation
* Technical documentation and architecture design

---

## Architecture Diagram

<img width="975" height="663" alt="image" src="https://github.com/user-attachments/assets/6cc36914-20cd-4f2c-a5aa-90af6e93c6b1" />

---

## Key AWS Components

The project includes screenshots demonstrating:

### Amazon Cognito Authentication
![Cognito Authentication](Screenshots/cognito.png)

### Amazon API Gateway
![API Gateway](Screenshots/API-Gateway.png) 

### AWS Lambda Functions
![Lambda Functions](Screenshots/Lambda-Functions.png)

### Amazon CloudWatch Monitoring
![CloudWatch Monitoring](Screenshots/CloudWatch-Logs.png)

### Amazon CloudFront Distribution
![CloudFront Distribution](Screenshots/CloudFront-Distro.png)

---

## Future Improvements

Potential future enhancements include:

* Web Application Firewall (AWS WAF) integration
* Expanded monitoring dashboards
* Centralized SIEM ingestion workflows
* CI/CD pipeline hardening
* Enhanced infrastructure automation
* Advanced alerting and operational analytics
