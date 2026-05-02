---
title: "Week 6 Worklog"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Objectives of Week 6

* Set up system monitoring for the entire application.
* Perform performance and stability testing.
* Start controlling operational costs on AWS.

---

### Tasks Completed During the Week

| Day | Task | Start Date | End Date | References |
|-----|------|------------|----------|------------|
| 1 | - Perform stress testing <br>&emsp; + Test ALB and ECS under high load <br>&emsp; + Record performance metrics | 13/04/2026 | 13/04/2026 | - |
| 2 | - Set up Amazon CloudWatch <br>&emsp; + Collect logs and metrics <br>&emsp; + Monitor CPU, memory, and requests | 14/04/2026 | 14/04/2026 | - |
| 3 | - Build monitoring dashboard <br>&emsp; + Aggregate key metrics <br>&emsp; + Visualize system performance | 15/04/2026 | 15/04/2026 | - |
| 4 | - Configure cost alerts <br>&emsp; + Set up budget alarms <br>&emsp; + Receive notifications when exceeding thresholds | 16/04/2026 | 16/04/2026 | - |
| 5 | - Optimize logging <br>&emsp; + Adjust log retention policy <br>&emsp; + Reduce CloudWatch Logs costs | 17/04/2026 | 17/04/2026 | - |
| 6 | - Create operational runbook <br>&emsp; + Document incident handling procedures <br>&emsp; + Define service restart workflows | 18/04/2026 | 18/04/2026 | - |
| 7 | - System validation <br>&emsp; + Evaluate performance after optimizations <br>&emsp; + Prepare for security hardening phase | 19/04/2026 | 19/04/2026 | - |

---

### Weekly Achievements

* A complete monitoring system is established for real-time observability.
* Baseline performance metrics have been defined.
* Cost monitoring is enabled with automated alerts.

---

### Challenges & Lessons Learned

* **Challenge:** CloudWatch Logs costs increased quickly due to default retention settings.
* **Solution:** Adjust log retention policies and optimize logging configuration.
* **Lesson Learned:** Monitoring is not only for detecting issues but also for controlling operational costs.

---

### Plan for Next Week

* Strengthen system security using AWS WAF.
* Set up a Bastion Host for secure access.
* Automate backend workflows.