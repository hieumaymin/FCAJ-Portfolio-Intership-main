---
title: "Week 3 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Objectives of Week 3

* Finalize functional requirements and non-functional requirements (NFR) for the Spendwise application.
* Initialize infrastructure management using Terraform (S3 backend and state strategy).
* Set up core AWS infrastructure including VPC, Security Groups, ALB, and ECR.

---

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Analyze Spendwise requirements <br>&emsp; + Define expense tracking and financial analysis features <br>&emsp; + Identify system stability and data security requirements | 23/03/2026 | 23/03/2026 | - |
| 2 | - Initialize Terraform <br>&emsp; + Configure S3 bucket as remote backend <br>&emsp; + Set up DynamoDB for state locking | 24/03/2026 | 24/03/2026 | - |
| 3 | - Set up Amazon VPC <br>&emsp; + Create Public and Private Subnets across multiple Availability Zones <br>&emsp; + Configure Internet Gateway for public access | 25/03/2026 | 25/03/2026 | - |
| 4 | - Configure security <br>&emsp; + Create Security Groups for ALB, ECS, and RDS <br>&emsp; + Apply least privilege principle | 26/03/2026 | 26/03/2026 | - |
| 5 | - Initialize compute services <br>&emsp; + Create repository on Amazon ECR <br>&emsp; + Configure basic ECS Cluster | 27/03/2026 | 27/03/2026 | - |
| 6 | - Set up load balancing <br>&emsp; + Configure Application Load Balancer (ALB) <br>&emsp; + Create Target Group for backend (NestJS) | 28/03/2026 | 28/03/2026 | - |
| 7 | - Infrastructure validation <br>&emsp; + Verify connectivity between subnets <br>&emsp; + Test pushing Docker images to ECR | 29/03/2026 | 29/03/2026 | - |

---

### Weekly Achievements

* Finalized system requirements and defined a clear 3-tier architecture on AWS.
* Successfully established VPC infrastructure with proper Public/Private segmentation.
* Configured Security Groups for different services following best practices.
* Set up Amazon ECR as a container image repository.
* Deployed Application Load Balancer as the entry point for the system.
* Initialized Terraform for Infrastructure as Code (IaC) management.

---

### Challenges & Lessons Learned

* **Challenge:** Designing subnet structure and routing while ensuring internal traffic does not go through the Internet.
* **Solution:** Follow AWS VPC best practices and clearly separate Public and Private layers.
* **Lesson Learned:** Using Terraform from the beginning helps manage infrastructure efficiently and enables easy reuse across environments.

---

### Plan for Next Week

* Integrate authentication using Amazon Cognito.
* Push backend Docker image to ECR and deploy on ECS Fargate.
* Connect frontend (Amplify) with real backend API endpoints.