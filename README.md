


# Dynamic Website on AWS - DevOps Project

## Overview
This project involves hosting a dynamic website on Amazon Web Services (AWS) utilizing various cloud resources to ensure high availability, scalability, and security. The architecture is designed to leverage AWS services effectively, providing a robust solution for web hosting.

## Repository
You can find the reference diagram and deployment scripts in the [GitHub Repository](#)  

## Architecture
The architecture consists of a Virtual Private Cloud (VPC) configured with both public and private subnets across two availability zones. This setup enhances system reliability and fault tolerance.

### Key Components
1. Virtual Private Cloud (VPC): Configured with public and private subnets spanning two availability zones.
2. Internet Gateway: Deployed to enable connectivity between VPC instances and the wider internet.
3. Security Groups: Established as a network firewall mechanism to control inbound and outbound traffic.
4. Availability Zones: Leveraged to increase system reliability and fault tolerance.
5. Public Subnets: Used for infrastructure components such as the NAT Gateway and Application Load Balancer.
6. EC2 Instance Connect Endpoint: Implemented for secure connections to assets within both public and private subnets.
7. Web Servers (EC2 Instances): Placed within private subnets for enhanced security.
8. NAT Gateway: Allowed instances in both the private Application and Data subnets to access the internet.
9. Application Load Balancer: Used to distribute web traffic evenly to an Auto Scaling Group of EC2 instances across multiple Availability Zones.
10. Auto Scaling Group: Automatically manages EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.
11. Certificate Manager: Secured application communications.
12. Simple Notification Service (SNS): Configured to alert about activities within the Auto Scaling Group.
13. Domain Registration and DNS: Registered the domain name and set up a DNS record using Route 53.
14. S3 Storage: Application codes are stored in Amazon S3 for easy access and management.

## Getting Started
To deploy this project, follow these steps:

1. Clone the repository:

bash
   git clone 
   


2. Navigate to the project directory:

bash
   cd 
   


3. Review the deployment scripts and reference diagram provided in the repository.

4. Ensure you have the necessary AWS permissions and configurations set up in your AWS account.

5. Execute the deployment scripts to provision the resources as per the architecture.
