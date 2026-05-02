---
title: "Week 5 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Objectives of Week 5

* Deploy the database on AWS.
* Secure sensitive system information.
* Configure HTTPS and a custom domain for the application.

---

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Initialize Amazon RDS (PostgreSQL) <br>&emsp; + Deploy in Private Subnet <br>&emsp; + Configure appropriate instance type | 06/04/2026 | 06/04/2026 | - |
| 2 | - Perform database migration <br>&emsp; + Connect ECS Service to RDS <br>&emsp; + Apply database schema | 07/04/2026 | 07/04/2026 | - |
| 3 | - Set up AWS Secrets Manager <br>&emsp; + Store database credentials securely <br>&emsp; + Remove hardcoded secrets from source code | 08/04/2026 | 08/04/2026 | - |
| 4 | - Configure VPC Endpoint <br>&emsp; + Gateway Endpoint for S3 <br>&emsp; + Optimize internal traffic routing | 09/04/2026 | 09/04/2026 | - |
| 5 | - Configure HTTPS <br>&emsp; + Request SSL certificate via ACM <br>&emsp; + Attach certificate to ALB | 10/04/2026 | 10/04/2026 | - |
| 6 | - Configure custom domain <br>&emsp; + Map domain using Route 53 <br>&emsp; + Connect to ALB and Amplify | 11/04/2026 | 11/04/2026 | - |
| 7 | - Perform security audit <br>&emsp; + Close unnecessary ports <br>&emsp; + Review Security Group rules | 12/04/2026 | 12/04/2026 | - |

---

### Weekly Achievements

* Database is running reliably within a private network.
* Sensitive information is securely managed using AWS Secrets Manager.
* The system now supports HTTPS with a custom domain.

---

### Challenges & Lessons Learned

* **Challenge:** Managing connections between ECS and RDS to avoid database overload.
* **Solution:** Monitor connection usage and apply controlled migration strategies.
* **Lesson Learned:** Security should be implemented from the early stages, not as an afterthought.

---

### Plan for Next Week

* Set up system monitoring using CloudWatch.
* Perform performance testing.
* Configure cost monitoring and alerts.