---
title: "Week 4 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Objectives of Week 4

* Initialize infrastructure using Terraform.
* Set up core networking components on AWS.
* Prepare the foundation for application deployment.

---

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Initialize Terraform <br>&emsp; + Configure S3 bucket as remote backend <br>&emsp; + Set up DynamoDB for state locking | 30/03/2026 | 30/03/2026 | [Terraform Remote State](https://developer.hashicorp.com/terraform/language/settings/backends/s3), [DynamoDB Lock](https://developer.hashicorp.com/terraform/language/settings/backends/s3#dynamodb-state-locking) |
| 2 | - Set up Amazon VPC <br>&emsp; + Create Public and Private Subnets across multiple Availability Zones <br>&emsp; + Configure Internet Gateway for public access | 31/03/2026 | 31/03/2026 | [VPC Subnets Guide](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html), [Internet Gateways](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html) |
| 3 | - Configure security <br>&emsp; + Create Security Groups for ALB, ECS, and RDS <br>&emsp; + Apply least privilege principle | 01/04/2026 | 01/04/2026 | [Security Group Best Practices](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html), [ECS Security](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security.html) |
| 4 | - Initialize container services <br>&emsp; + Create repository on Amazon ECR <br>&emsp; + Configure basic ECS Cluster | 02/04/2026 | 02/04/2026 | [ECR Repository Guide](https://docs.aws.amazon.com/AmazonECR/latest/userguide/Repositories.html), [ECS Cluster Setup](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create_cluster.html) |
| 5 | - Set up load balancing <br>&emsp; + Configure Application Load Balancer (ALB) <br>&emsp; + Create Target Group for backend service | 03/04/2026 | 03/04/2026 | [ALB Target Groups](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html), [ALB Listeners](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-listeners.html) |
| 6 | - Configure VPC Endpoints <br>&emsp; + Interface Endpoints for ECR and CloudWatch <br>&emsp; + Ensure internal traffic does not go through the Internet | 04/04/2026 | 04/04/2026 | [AWS PrivateLink (Interface Endpoints)](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints.html), [ECR VPC Endpoints](https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html) |
| 7 | - Infrastructure validation <br>&emsp; + Verify connectivity between subnets <br>&emsp; + Test internal access via VPC Endpoints | 05/04/2026 | 05/04/2026 | - |

---

### Weekly Achievements

* Core networking infrastructure (VPC) was successfully established with clear Public/Private segmentation.
* Terraform was fully utilized to manage infrastructure as code.
* Foundational services such as ECR, ECS, and ALB were ready for deployment.

---

### Challenges & Lessons Learned

* **Challenge:** Designing VPC and configuring routing rules was initially complex.
* **Solution:** Follow AWS best practices and validate each component step-by-step.
* **Lesson Learned:** A well-designed infrastructure foundation significantly reduces future scalability and maintenance issues.

---

### Plan for Next Week

* Deploy backend application to ECS Fargate.
* Integrate user authentication using Amazon Cognito.
* Connect frontend with backend APIs.
