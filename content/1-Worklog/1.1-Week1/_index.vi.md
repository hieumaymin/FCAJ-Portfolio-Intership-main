---
title: "Worklog Tuần 1"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu Tuần 1

* Hiểu các khái niệm cơ bản về điện toán đám mây và hạ tầng toàn cầu của AWS.
* Học cách quản lý các dịch vụ AWS bằng Management Console, CLI và SDK.
* Tìm hiểu về bảo mật AWS, IAM và quản lý chi phí.
* Xây dựng kiến thức nền tảng về mạng VPC và kết nối.
* Có kinh nghiệm thực hành thông qua các bài lab AWS.

---

### Công việc đã thực hiện trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|------|-----------|--------------|---------------|---------------------|
| 1 | - Nghiên cứu kiến thức cơ bản về cloud <br>&emsp; + Hạ tầng AWS (Region, AZ, Edge Location) <br>&emsp; + Mô hình giá và gói hỗ trợ AWS <br>&emsp; + Thực hành: bảo mật Root User, cấu hình IAM (User, Group, MFA), tạo AWS Budgets | 09/03/2026 | 09/03/2026 | [Cloud Essentials, IAM Docs](https://explore.skillbuilder.aws/learn/course/external/view/elearning/134/aws-cloud-practitioner-essentials) |
| 2 | - Tìm hiểu kiến trúc VPC <br>&emsp; + CIDR và địa chỉ IP <br>&emsp; + Subnet Public/Private <br>&emsp; + Route Table, IGW, NAT Gateway <br>&emsp; + Elastic IP, ENI, VPC Endpoint | 10/03/2026 | 10/03/2026 | [VPC User Guide, Subnet Calc](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| 3 | - Nghiên cứu bảo mật và kết nối mạng <br>&emsp; + Security Group vs Network ACL <br>&emsp; + Giám sát bằng VPC Flow Logs <br>&emsp; + VPC Peering, Transit Gateway <br>&emsp; + VPN và Direct Connect <br>&emsp; + Elastic Load Balancer (ALB, NLB, GWLB) | 11/03/2026 | 11/03/2026 | [VPC Security, ELB Docs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html) |
| 4 | - Lab thực hành: triển khai VPC <br>&emsp; + Tạo VPC, Subnet, Route Table, IGW <br>&emsp; + Khởi tạo EC2 <br>&emsp; + Cấu hình NAT Gateway cho private subnet <br>&emsp; + Giám sát bằng CloudWatch <br>&emsp; + Sử dụng SSM Session Manager | 12/03/2026 | 12/03/2026 | [Session Manager, NAT Gateway](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager.html) |
| 5 | - Lab thực hành: mạng nâng cao <br>&emsp; + Thực hành Port Forwarding với Session Manager <br>&emsp; + Cấu hình VPC Peering (cross-region/account) <br>&emsp; + Triển khai Transit Gateway (hub-and-spoke) <br>&emsp; + Cấu hình Route 53 Resolver cho Hybrid DNS | 13/03/2026 | 13/03/2026 | [VPC Peering, Transit Gateway](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) |
| 6 | - Ôn tập và củng cố kiến thức <br>&emsp; + Ôn lại IAM, VPC, Security <br>&emsp; + Làm thêm lab AWS | 14/03/2026 | 14/03/2026 | [AWS Ramp-Up Guide](https://d1.awsstatic.com/training-and-certification/ramp-up-guides/Ramp-Up_Guide_Architect.pdf) |
| 7 | - Tổng kết tuần <br>&emsp; + Ghi chú lại kiến thức <br>&emsp; + Chuẩn bị cho giai đoạn tiếp theo | 15/03/2026 | 15/03/2026 | - |

---

### Kết quả đạt được

* Nắm vững kiến thức cơ bản về cloud và AWS.
* Thực hành sử dụng AWS Management Console, CLI và SDK.
* Cấu hình IAM, MFA và AWS Budgets để kiểm soát chi phí.
* Xây dựng và cấu hình hệ thống mạng VPC.
* Triển khai bảo mật với Security Group và Network ACL.
* Thực hành lab với EC2, CloudWatch và Session Manager.
* Hiểu và áp dụng các mô hình mạng nâng cao (VPC Peering, Transit Gateway, Hybrid DNS, ELB).

---

### Khó khăn & Bài học kinh nghiệm

* **Khó khăn:** Khối lượng kiến thức AWS lớn và nhiều dịch vụ mới.
* **Giải pháp:** Kết hợp học lý thuyết với thực hành lab.
* **Bài học:** Thực hành là yếu tố quan trọng để hiểu rõ cloud và networking.

---

### Kế hoạch tuần tiếp theo

* Tiếp tục thực hành các lab AWS.
* Tập trung vào các dịch vụ compute và storage (EC2, S3, RDS).
* Bắt đầu xây dựng một ứng dụng nhỏ trên cloud.