---
title: "Worklog Tuần 3"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3

* Chốt yêu cầu chức năng và các yêu cầu phi chức năng (NFR) cho ứng dụng Spendwise.
* Khởi tạo quản lý hạ tầng bằng Terraform (S3 backend và chiến lược state).
* Thiết lập hạ tầng AWS cơ bản gồm VPC, Security Groups, ALB và ECR.

---

### Công việc đã thực hiện trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|------|-----------|--------------|---------------|---------------------|
| 1 | - Phân tích yêu cầu hệ thống Spendwise <br>&emsp; + Xác định chức năng theo dõi và phân tích chi tiêu <br>&emsp; + Định nghĩa yêu cầu về độ ổn định và bảo mật dữ liệu | 23/03/2026 | 23/03/2026 | [AWS Cloud Adoption Framework](https://aws.amazon.com/caf/), [FinOps Principles](https://www.finops.org/introduction/what-is-finops/) |
| 2 | - Khởi tạo Terraform <br>&emsp; + Cấu hình S3 bucket làm remote backend <br>&emsp; + Thiết lập DynamoDB để lock state | 24/03/2026 | 24/03/2026 | [Terraform S3 Backend Guide](https://developer.hashicorp.com/terraform/language/settings/backends/s3), [State Locking with DynamoDB](https://developer.hashicorp.com/terraform/language/settings/backends/s3#dynamodb-state-locking) |
| 3 | - Thiết lập Amazon VPC <br>&emsp; + Tạo Subnet Public/Private trên nhiều Availability Zones <br>&emsp; + Cấu hình Internet Gateway cho lớp Public | 25/03/2026 | 25/03/2026 | [VPC Multi-AZ Architecture](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-subnets-plans.html), [Terraform VPC Module](https://registry.terraform.io/modules/terraform-aws-modules/vpc/aws/latest) |
| 4 | - Cấu hình bảo mật <br>&emsp; + Tạo Security Groups cho ALB, ECS và RDS <br>&emsp; + Áp dụng nguyên tắc Least Privilege | 26/03/2026 | 26/03/2026 | [Security Group Rules](https://docs.aws.amazon.com/vpc/latest/userguide/security-group-rules.html), [IAM Least Privilege Principle](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege) |
| 5 | - Khởi tạo dịch vụ compute <br>&emsp; + Tạo repository trên Amazon ECR <br>&emsp; + Cấu hình ECS Cluster cơ bản | 27/03/2026 | 27/03/2026 | [Amazon ECR User Guide](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html), [ECS Cluster Concepts](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/clusters.html) |
| 6 | - Cấu hình cân bằng tải <br>&emsp; + Thiết lập Application Load Balancer (ALB) <br>&emsp; + Tạo Target Group cho backend (NestJS) | 28/03/2026 | 28/03/2026 | [ALB Components](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html#application-load-balancer-components), [NestJS on AWS Guide](https://docs.nestjs.com/deployment/aws) |
| 7 | - Kiểm tra hạ tầng <br>&emsp; + Kiểm tra kết nối giữa các subnet <br>&emsp; + Test push Docker image lên ECR | 29/03/2026 | 29/03/2026 | - |

---

### Kết quả đạt được

* Hoàn thiện yêu cầu hệ thống và xác định rõ kiến trúc 3-tier trên AWS.
* Thiết lập thành công hạ tầng mạng VPC với phân tách Public/Private rõ ràng.
* Cấu hình Security Groups theo best practice cho từng dịch vụ.
* Tạo và sử dụng Amazon ECR làm nơi lưu trữ Docker image.
* Triển khai Application Load Balancer làm điểm truy cập hệ thống.
* Áp dụng Terraform để quản lý hạ tầng dưới dạng code (IaC).

---

### Khó khăn & Bài học kinh nghiệm

* **Khó khăn:** Thiết kế subnet và routing phức tạp, đặc biệt khi đảm bảo traffic nội bộ không đi qua Internet.
* **Giải pháp:** Áp dụng best practices của AWS và tách biệt rõ ràng Public/Private.
* **Bài học:** Sử dụng Terraform ngay từ đầu giúp quản lý hạ tầng hiệu quả và dễ tái sử dụng.

---

### Kế hoạch tuần tiếp theo

* Tích hợp xác thực người dùng với Amazon Cognito.
* Đẩy Docker image của backend lên ECR và deploy trên ECS Fargate.
* Kết nối frontend (Amplify) với API backend thực tế.