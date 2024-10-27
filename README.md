# Secure AWS Environment Project
=====================================

## Objective
---------------

This project demonstrates the setup of a secure AWS environment using Free Tier resources, covering VPC, subnets, Internet Gateway, EC2 instances, security groups, IAM users and roles, CloudTrail, GuardDuty and a Lambda function for incident response automation.

### Skills Learned
--------------------

* AWS cloud security fundamentals
* VPC and subnet configuration
* EC2 instance deployment and security
* IAM user and role management
* CloudTrail and GuardDuty setup
* Lambda function automation

### Tools Used
----------------

* AWS Management Console
* AWS Cloud Development Kit (CDK)
* AWS Infrastructure Composer
* EC2 instances (Web and Database servers)
* Security Groups
* IAM (Identity and Access Management)
* CloudTrail
* GuardDuty
* Lambda Function


## Architecture Diagram
----------------------

### Overview

The architecture consists of:

*   1 VPC with 2 subnets (public and private)
*   1 Internet Gateway
*   2 EC2 instances (web server and database server)
*   2 Security Groups
*   1 IAM user and role
*   CloudTrail and GuardDuty for logging and threat detection
*   1 Lambda function for automated incident response

### Architecture Components

Architecture Diagram


![FinalArchitecture](https://github.com/user-attachments/assets/f006b84b-6903-40b0-8973-5b20a1b07fea)


## Steps
------------


### 1. VPC Creation

Setting up a Virtual Private Cloud (VPC) with IPv4 CIDR block 10.0.0.0/16.


![VPC](https://github.com/user-attachments/assets/9b15efe7-c3dd-4dfd-b882-4282e0d968a3)


### 2. Public Subnet and Private Subnet Creation



![Subnet](https://github.com/user-attachments/assets/cc1faeaf-c28d-4b9b-88b1-446ae51e8f4a)



### 3. Internet Gateway Creation

Creating an Internet Gateway and attaching it to the VPC.


![AppGateway](https://github.com/user-attachments/assets/13557d5f-eaba-4444-9825-1c573e0ea48d)



![AttachVpc](https://github.com/user-attachments/assets/8a1bcad9-81d3-48ae-a7c0-ff8e6683cd31)

### 4. EC2 Instance (Web Server, Database Server) Creation

Launching a web server, Database Server EC2 instance with Public and Private Subnet Associations for secure access.


![LaunchInstance](https://github.com/user-attachments/assets/628dfa6d-187d-4665-b526-a3b4a7f008e2)


![DBServerConfig](https://github.com/user-attachments/assets/1ef10cef-53b1-40ac-9dc9-0678f9e3be5b)


![SubnetAssociations](https://github.com/user-attachments/assets/22884700-49a9-486a-a2c5-2d989c30569a)



### 5. Security Group Configuration

Configuring security groups for web and database servers.

![securityGroup](https://github.com/user-attachments/assets/7d714c4b-7d8a-4407-8444-f2f35cccc967)



### 6. IAM User and Role Creation

Creating an IAM user and role for secure access.


![IAMUser](https://github.com/user-attachments/assets/aaacecb0-9106-4932-b48a-7f78411397a2)


### 7. CloudTrail Setup

Enabling CloudTrail for logging and monitoring.


![CloudTrail](https://github.com/user-attachments/assets/afdd1729-829d-4595-b8bf-166c4e5a508d)


### 8. GuardDuty Setup

Enabling GuardDuty for threat detection.


![GuardDuty](https://github.com/user-attachments/assets/183df7c1-429a-4a50-9c34-1bc9b4b6ff58)


### 9. Lambda Function Creation

Creating a Lambda function for automated incident response.


![LamdaFunc](https://github.com/user-attachments/assets/2b4115bc-12b1-46d0-954f-fbe70db14c25)



## Conclusion
--------------
### GuardDuty Findings

![GuardDutyFindings](https://github.com/user-attachments/assets/62a2b753-e74c-4c7c-9ed3-2c52889c743f)


### CloudTrail Findings

![CloudTrailFindings](https://github.com/user-attachments/assets/14c639fe-f31d-471a-9a6b-7b60f9132341)


### Testing Lamda Function for account compromise

![LambdaFunc](https://github.com/user-attachments/assets/9c40d6b6-1021-4090-92c5-6b4cdec5f70e)


This project demonstrates a secure AWS environment setup using Free Tier resources, covering key cloud security concepts and services.
