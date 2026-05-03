---
title: "Week 7 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Objectives of Week 7

* Optimize system performance based on real usage data.
* Implement auto-scaling for dynamic workload handling.
* Analyze and reduce operational costs.

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Analyze system resource usage <br>&emsp; + Monitor CPU and memory metrics of ECS <br>&emsp; + Evaluate real usage patterns | 20/04/2026 | 20/04/2026 | [ECS CloudWatch Metrics](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-metrics.html), [Compute Optimizer Guide](https://docs.aws.amazon.com/compute-optimizer/latest/ug/what-is-compute-optimizer.html) |
| 2 | - Optimize ECS tasks <br>&emsp; + Adjust CPU/RAM allocation (right-sizing) <br>&emsp; + Reduce over-provisioning | 21/04/2026 | 21/04/2026 | [ECS Task Definition Parameters](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#task_size), [Right-sizing AWS Resources](https://aws.amazon.com/aws-cost-management/aws-cost-optimization/right-sizing/) |
| 3 | - Implement auto-scaling <br>&emsp; + Configure scaling policies based on ALB requests <br>&emsp; + Test scale in/out behavior | 22/04/2026 | 22/04/2026 | [ECS Service Auto Scaling](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-auto-scaling.html), [Target Tracking Scaling Policies](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-target-tracking.html) |
| 4 | - Log analysis <br>&emsp; + Use CloudWatch Logs Insights <br>&emsp; + Create queries to track 5xx errors | 23/04/2026 | 23/04/2026 | [CloudWatch Logs Insights Syntax](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html), [Analyzing ALB Access Logs](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-access-logs.html) |
| 5 | - Resilience testing <br>&emsp; + Simulate service crashes <br>&emsp; + Observe ECS self-healing behavior | 24/04/2026 | 24/04/2026 | [AWS Fault Injection Service](https://aws.amazon.com/fis/), [ECS Service Deployment Health](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-circuit-breaker.html) |
| 6 | - Network cost optimization <br>&emsp; + Evaluate NAT Gateway usage <br>&emsp; + Compare with VPC Endpoints | 25/04/2026 | 25/04/2026 | [Reducing NAT Gateway Costs](https://aws.amazon.com/blogs/networking-and-content-delivery/how-to-reduce-costs-for-nat-gateway-usage/), [VPC Endpoint Pricing](https://aws.amazon.com/privatelink/pricing/) |
| 7 | - Resource cleanup <br>&emsp; + Configure ECR lifecycle policy <br>&emsp; + Remove unused resources | 26/04/2026 | 26/04/2026 | [ECR Lifecycle Policies](https://docs.aws.amazon.com/AmazonECR/latest/userguide/LifecyclePolicies.html), [Terraform Lifecycle Management](https://developer.hashicorp.com/terraform/language/resources/lifecycle) |

### Weekly Achievements

* The system can automatically scale based on traffic demand.
* Resource usage is optimized, reducing unnecessary costs.
* Improved observability through better log analysis.

### Challenges & Lessons Learned

* **Challenge:** Determining optimal scaling thresholds initially.
* **Solution:** Continuously monitor real data and adjust incrementally.
* **Lesson Learned:** Optimization is an ongoing process driven by real metrics, not assumptions.

### Plan for Next Week

* Finalize system documentation (As-built architecture).
* Perform disaster recovery testing.
* Prepare for project handover and final presentation.