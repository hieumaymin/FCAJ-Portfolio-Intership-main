---
title: "Week 2 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Objectives of Week 2

* Learn and practice AWS Compute services (EC2, AMI, EBS, Auto Scaling, ELB).
* Gain experience in monitoring and backup using CloudWatch and AWS Backup.
* Explore AWS Storage services (S3, Storage Gateway, FSx).
* Perform hands-on deployment, scaling, and static website hosting.

---

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Study AWS Compute & EC2 <br>&emsp; + EC2 architecture, instance types, pricing (On-demand, Spot, Reserved) <br>&emsp; + AMI, Snapshot, EBS vs Instance Store <br>&emsp; + Launch EC2 (Linux & Windows) <br>&emsp; + Connect via SSH and RDP <br>&emsp; + Deploy Node.js CRUD application on EC2 | 16/03/2026 | 16/03/2026 | [EC2 User Guide](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html), [EBS vs Instance Store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html) |
| 2 | - High availability & monitoring <br>&emsp; + Configure Auto Scaling Group <br>&emsp; + Set up Elastic Load Balancer (ELB) <br>&emsp; + Monitor using CloudWatch (metrics, logs, alarms) <br>&emsp; + Configure AWS Backup for EC2 and related services | 17/03/2026 | 17/03/2026 | [Auto Scaling Guide](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html), [CloudWatch Logs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html) |
| 3 | - Learn Amazon S3 <br>&emsp; + S3 architecture and object storage <br>&emsp; + Storage classes (Standard, IA, Glacier) <br>&emsp; + Configure Bucket Policy, ACL, Versioning <br>&emsp; + Lifecycle and data archiving | 18/03/2026 | 18/03/2026 | [S3 Storage Classes](https://aws.amazon.com/s3/storage-classes/), [S3 Lifecycle Management](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html) |
| 4 | - Hybrid storage with Storage Gateway <br>&emsp; + Overview of hybrid cloud storage <br>&emsp; + Deploy File Gateway on EC2 <br>&emsp; + Configure NFS File Share linked to S3 <br>&emsp; + Mount storage from local machine | 19/03/2026 | 19/03/2026 | [Storage Gateway Guide](https://docs.aws.amazon.com/storagegateway/latest/userguide/WhatIsStorageGateway.html), [File Gateway Setup](https://docs.aws.amazon.com/storagegateway/latest/userguide/CreatingAnS3FileGateway.html) |
| 5 | - Managed storage & hosting <br>&emsp; + Deploy Amazon FSx for Windows File Server <br>&emsp; + Configure shared file system (SMB) <br>&emsp; + Host static website using S3 <br>&emsp; + Configure CloudFront and OAI for secure delivery | 20/03/2026 | 20/03/2026 | [Amazon FSx Guide](https://docs.aws.amazon.com/fsx/latest/WindowsGuide/what-is.html), [CloudFront OAC/OAI](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html) |
| 6 | - Review & practice <br>&emsp; + Revisit EC2, S3, Auto Scaling <br>&emsp; + Practice additional labs and deployment scenarios | 21/03/2026 | 21/03/2026 | [AWS Architecture Center](https://aws.amazon.com/architecture/), [AWS Self-Paced Labs](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/) |
| 7 | - Validate & summarize <br>&emsp; + Test scaling and load balancing <br>&emsp; + Verify monitoring and backup system <br>&emsp; + Summarize knowledge and prepare next phase | 22/03/2026 | 22/03/2026 | - |

---

### Weekly Achievements

* Gained solid understanding of EC2, AMI, EBS, and instance deployment.
* Successfully deployed and managed Linux & Windows EC2 instances.
* Implemented Auto Scaling and Elastic Load Balancer for high availability.
* Monitored systems using CloudWatch (metrics, logs, alarms).
* Configured AWS Backup for automated data protection.
* Learned and applied Amazon S3 (storage classes, lifecycle, access control).
* Implemented static website hosting with S3 and CloudFront.
* Explored hybrid storage (Storage Gateway) and managed file systems (FSx).

---

### Challenges & Lessons Learned

* **Challenge:** Managing multiple AWS services and understanding their integration.
* **Solution:** Practice through hands-on labs and follow AWS architecture patterns.
* **Lesson Learned:** Combining compute, storage, and monitoring is key to building reliable cloud systems.

---

### Plan for Next Week

* Finalize Spendwise functional requirements and Non-Functional Requirements (NFRs).
* Implement Terraform management strategy, including S3 backend and state locking.

