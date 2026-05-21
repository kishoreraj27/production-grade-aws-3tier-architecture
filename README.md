\# Production-Grade AWS 3-Tier Architecture



\## Project Overview



This project demonstrates the deployment of a production-grade 3-tier web architecture on AWS using secure networking, scalable infrastructure, load balancing, and automated EC2 provisioning.



The architecture follows enterprise cloud design principles including:



\- Public and Private Subnet Isolation

\- Bastion Host Access

\- NAT Gateway for Private Internet Access

\- Application Load Balancer (ALB)

\- Auto Scaling Group (ASG)

\- Private RDS MySQL Database

\- Infrastructure Automation using Launch Templates and User Data



\---



\# Architecture Diagram



!\[Architecture Diagram](architecture-diagram/aws-3tier-architecture-diagram.png)



\---



\# Architecture Flow



```text

Internet

&#x20;  ↓

Public Application Load Balancer

&#x20;  ↓

Auto Scaling Group (Private EC2 Instances)

&#x20;  ↓

RDS MySQL Database

```



\---



\# AWS Services Used



| Service | Purpose |

|---|---|

| VPC | Isolated cloud network |

| Public \& Private Subnets | Secure tier separation |

| Internet Gateway | Public internet access |

| NAT Gateway | Outbound internet for private instances |

| Security Groups | Stateful firewall protection |

| Bastion Host | Secure SSH access |

| EC2 | Application hosting |

| Application Load Balancer | Traffic distribution |

| Auto Scaling Group | High availability \& self-healing |

| Launch Template | Automated EC2 provisioning |

| RDS MySQL | Managed relational database |



\---



\# Key Features



\- Production-grade AWS architecture

\- Public and private subnet segmentation

\- Secure Bastion Host access

\- Private EC2 application deployment

\- Highly available Auto Scaling Group

\- Application Load Balancer integration

\- Automated EC2 provisioning using User Data

\- Private RDS database deployment

\- Responsive frontend application

\- Health check monitoring



\---



\# Project Screenshots



\## VPC Architecture



!\[VPC](screenshots/01-vpc-overview.png)



\---



\## Subnet Architecture



!\[Subnets](screenshots/02-subnet-architecture.png)



\---



\## Route Tables



!\[Route Tables](screenshots/03-route-tables.png)



\---



\## Security Groups



!\[Security Groups](screenshots/04-security-groups.png)



\---



\## NAT Gateway



!\[NAT Gateway](screenshots/05-nat-gateway.png)



\---



\## Private Server SSH Access



!\[SSH](screenshots/06-private-server-ssh.png)



\---



\## RDS MySQL Database



!\[RDS](screenshots/08-rds-private-mysql-instance.png)



\---



\## Internal Load Balancer



!\[Internal ALB](screenshots/10-internal-alb.png)



\---



\## Flask Application Health Check



!\[Health Check](screenshots/12-flask-app-alb-health-check.png)



\---



\## Public Load Balancer



!\[Public ALB](screenshots/17-public-alb.png)



\---



\## Frontend Application



!\[Frontend](screenshots/19-production-frontend-ui.png)



\---



\## Auto Scaling Group



!\[ASG](screenshots/21-auto-scaling-group-working.png)



\---



\# Application Deployment



The Flask application was deployed on private EC2 instances using:



\- Python3

\- Flask

\- User Data automation

\- Launch Templates

\- Auto Scaling Group



The application is served behind an Application Load Balancer for scalability and high availability.



\---



\# Security Implementation



This project follows secure cloud architecture best practices:



\- Private EC2 instances without public IP

\- RDS deployed in private subnets

\- Security Group referencing

\- Bastion Host controlled SSH access

\- NAT Gateway for outbound-only internet access

\- Application Load Balancer traffic filtering



\---



\# Auto Scaling Implementation



The project includes:



\- Launch Template configuration

\- Auto Scaling Group integration

\- Automatic EC2 provisioning

\- Health check monitoring

\- Multi-instance backend deployment



This ensures:

\- high availability

\- scalability

\- self-healing infrastructure



\---



\# Technologies Used



\- AWS VPC

\- EC2

\- RDS MySQL

\- Application Load Balancer

\- Auto Scaling Group

\- Launch Templates

\- NAT Gateway

\- Amazon Linux 2023

\- Python3

\- Flask

\- HTML

\- CSS



\---



\# Learning Outcomes



Through this project, I gained hands-on experience with:



\- AWS networking

\- VPC design

\- Public and private architecture

\- Load balancing

\- Auto Scaling

\- Infrastructure automation

\- Bastion architecture

\- Secure cloud deployment

\- High availability design

\- Cloud troubleshooting



\---



\# Future Enhancements



\- HTTPS with ACM

\- Route53 custom domain

\- CI/CD pipeline integration

\- Docker containerization

\- Terraform Infrastructure as Code

\- CloudWatch monitoring

\- WAF integration



\---



\# Author



\## Kishore Raj



AWS Cloud \& DevOps Enthusiast



\---

