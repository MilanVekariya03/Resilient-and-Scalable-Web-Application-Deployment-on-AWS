# Resilient-and-Scalable-Web-Application-Deployment-on-AWS

Project Overview

This project demonstrates the design and deployment of a highly available, scalable, secure, and fault-tolerant web application infrastructure on Amazon Web Services (AWS). The main objective of this project was to build a cloud-based architecture capable of handling traffic spikes efficiently while ensuring minimal downtime and improved performance.

The infrastructure was designed using multiple AWS services such as Amazon EC2, VPC, Application Load Balancer (ALB), Auto Scaling Group, Amazon EFS, and Route 53. The project follows modern cloud architecture practices by distributing resources across multiple Availability Zones (AZs) to achieve high availability and resilience.

Project Objectives

The primary objectives of this project were:

To deploy a scalable web application infrastructure on AWS.
To achieve high availability using Multi-AZ deployment.
To implement load balancing for efficient traffic distribution.
To configure Auto Scaling for automatic resource management.
To provide secure network communication using VPC and Security Groups.
To implement shared scalable storage using Amazon EFS.
To improve fault tolerance and application reliability.
AWS Services Used
1. Amazon VPC (Virtual Private Cloud)

A custom VPC was created to provide a secure and isolated network environment for the application infrastructure.

Components Configured:
Public Subnets
Private Subnets
Internet Gateway
Route Tables
Security Groups
Purpose:
Secure communication between resources
Network isolation
Controlled inbound and outbound traffic
2. Amazon EC2

Amazon EC2 instances were used to host the web application.

Features:
Amazon Linux instances
Web server installation and configuration
Scalable compute resources
Custom AMI creation for Auto Scaling
Benefits:
Flexible compute capacity
Easy deployment and management
Reliable application hosting
3. Application Load Balancer (ALB)

The Application Load Balancer was configured to distribute incoming traffic across multiple EC2 instances.

Purpose:
Prevent server overload
Ensure high availability
Improve application performance
Features:
Health checks
Traffic distribution
Fault tolerance
4. Auto Scaling Group

Auto Scaling was implemented to automatically adjust the number of EC2 instances based on traffic demand.

Functions:
Automatically launch new instances during high traffic
Remove unused instances during low traffic
Maintain desired application performance
Advantages:
Improved scalability
Reduced downtime
Cost optimization
5. Amazon EFS (Elastic File System)

Amazon EFS was integrated to provide centralized shared storage for multiple EC2 instances.

Benefits:
Shared storage across servers
Scalable file system
High availability storage solution
Use Case:

All EC2 instances could access the same application data and files.

6. Amazon Route 53

Route 53 was used for domain management and DNS routing.

Functions:
Domain name resolution
Reliable DNS routing
Better accessibility for users
Architecture Workflow

The architecture flow of the project is:

User → Route 53 → Application Load Balancer → EC2 Instances → Amazon EFS

Workflow Explanation:
Users access the application using a domain name.
Route 53 routes the request to the Application Load Balancer.
The ALB distributes traffic across multiple EC2 instances.
EC2 instances process the requests.
Shared files and application data are stored in Amazon EFS.
Key Features of the Project
High Availability

Resources were deployed across multiple Availability Zones to minimize downtime.

Scalability

Auto Scaling dynamically adjusts infrastructure resources according to traffic demand.

Fault Tolerance

The ALB and Multi-AZ deployment ensure the application remains available even if one server fails.

Security

Security Groups, IAM roles, and private networking were implemented to secure the infrastructure.

Performance Optimization

Load balancing and Auto Scaling improved overall application performance and reliability.

Challenges Faced and Solutions
1. Traffic Spike Management
Challenge:

Handling sudden increases in user traffic without affecting application performance.

Solution:

Implemented Auto Scaling Groups to automatically launch additional EC2 instances when CPU utilization increased.

2. Load Distribution
Challenge:

Preventing overload on a single EC2 instance.

Solution:

Configured an Application Load Balancer to evenly distribute incoming traffic across all running instances.

3. Shared Storage Across Servers
Challenge:

Managing centralized storage for multiple EC2 instances.

Solution:

Integrated Amazon EFS to provide scalable shared storage accessible by all application servers.

4. High Availability Across Availability Zones
Challenge:

Ensuring application availability during server or AZ failure.

Solution:

Deployed infrastructure resources across multiple Availability Zones.

5. Security Configuration
Challenge:

Protecting the infrastructure from unauthorized access.

Solution:

Configured Security Groups, IAM policies, and secure VPC networking.

Results Achieved

The project successfully achieved the following outcomes:

✅ High Availability
✅ Automatic Scaling
✅ Secure Infrastructure
✅ Improved Fault Tolerance
✅ Efficient Traffic Distribution
✅ Centralized Shared Storage
✅ Better Performance and Reliability

Learning Outcomes

Through this project, I gained hands-on experience in:

AWS Cloud Architecture
EC2 Deployment
VPC Networking
Load Balancing
Auto Scaling
Cloud Security
Shared Storage Configuration
DNS Management using Route 53

This project helped me understand real-world cloud deployment strategies and best practices for designing scalable and resilient applications on AWS.

Future Enhancements

The project can be further improved by implementing:

CI/CD Pipeline Integration
CloudWatch Monitoring and Alerts
AWS WAF for enhanced security
RDS Database Integration
Docker Containerization
Kubernetes (EKS) Deployment
Conclusion

This project successfully demonstrated how AWS cloud services can be used together to create a resilient, scalable, secure, and highly available web application infrastructure. By implementing services like EC2, ALB, Auto Scaling, EFS, and Route 53, the project achieved better scalability, fault tolerance, and performance optimization while following cloud best practices.

project ppt = [AWS_Deployment_MilanVekariya.pptx](https://github.com/user-attachments/files/28182228/AWS_Deployment_MilanVekariya.pptx)

<img width="673" height="918" alt="Image" src="https://github.com/user-attachments/assets/fc420753-1557-4e6f-998d-cb0501ab5279" />

<img width="954" height="659" alt="Image" src="https://github.com/user-attachments/assets/02c9f4c9-c96b-44f5-aff4-1ebce18dd8d7" />

<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/a725ddcf-b7bc-40f8-b082-0da729e27f10" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/82675547-f0cb-47e0-a040-b224fc5d764b" />

<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/6ec3f30c-4d69-4ec2-b788-59519131df77" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/9459bce3-b0d7-48a9-88b1-75f52073c4f2" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/440838dd-5bcf-471b-8879-a16fcc2f4d25" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/9ee3b078-4f65-46ac-b44f-617383203a83" />

<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/b235cad5-3535-4112-bf5c-df8bb2ec0ab0" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/eea4b19f-7f97-4c84-a0f1-20f780ea9f04" />

<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/cd369199-6ec1-406d-b5d4-132510083c0f" />
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/e349007a-2d5b-4332-aafd-41311388e136" />



