---
title: "Worklog Tuần 4"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4

* Khởi tạo hạ tầng bằng Terraform.
* Thiết lập các thành phần mạng cơ bản trên AWS.
* Chuẩn bị nền tảng cho việc triển khai ứng dụng.

---

### Công việc đã thực hiện trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|------|-----------|--------------|---------------|---------------------|
| 1 | - Khởi tạo Terraform <br>&emsp; + Cấu hình S3 bucket làm remote backend <br>&emsp; + Thiết lập DynamoDB để lock state | 30/03/2026 | 30/03/2026 | [Terraform Remote State](https://developer.hashicorp.com/terraform/language/settings/backends/s3), [DynamoDB Lock](https://developer.hashicorp.com/terraform/language/settings/backends/s3#dynamodb-state-locking) |
| 2 | - Thiết lập Amazon VPC <br>&emsp; + Tạo Subnet Public/Private trên nhiều Availability Zones <br>&emsp; + Cấu hình Internet Gateway cho lớp Public | 31/03/2026 | 31/03/2026 | [VPC Subnets Guide](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html), [Internet Gateways](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html) |
| 3 | - Cấu hình bảo mật <br>&emsp; + Tạo Security Groups cho ALB, ECS và RDS <br>&emsp; + Áp dụng nguyên tắc Least Privilege | 01/04/2026 | 01/04/2026 | [Security Group Best Practices](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html), [ECS Security](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security.html) |
| 4 | - Khởi tạo dịch vụ container <br>&emsp; + Tạo repository trên Amazon ECR <br>&emsp; + Cấu hình ECS Cluster cơ bản | 02/04/2026 | 02/04/2026 | [ECR Repository Guide](https://docs.aws.amazon.com/AmazonECR/latest/userguide/Repositories.html), [ECS Cluster Setup](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create_cluster.html) |
| 5 | - Thiết lập cân bằng tải <br>&emsp; + Cấu hình Application Load Balancer (ALB) <br>&emsp; + Tạo Target Group cho backend service | 03/04/2026 | 03/04/2026 | [ALB Target Groups](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html), [ALB Listeners](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-listeners.html) |
| 6 | - Cấu hình VPC Endpoints <br>&emsp; + Thiết lập Interface Endpoints cho ECR và CloudWatch <br>&emsp; + Đảm bảo traffic nội bộ không đi qua Internet | 04/04/2026 | 04/04/2026 | [AWS PrivateLink (Interface Endpoints)](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints.html), [ECR VPC Endpoints](https://docs.aws.amazon.com/AmazonECR/latest/userguide/vpc-endpoints.html) |
| 7 | - Kiểm tra hạ tầng <br>&emsp; + Kiểm tra kết nối giữa các subnet <br>&emsp; + Test truy cập nội bộ thông qua VPC Endpoints | 05/04/2026 | 05/04/2026 | - |

---

### Kết quả đạt được

* Hạ tầng mạng (VPC) được thiết lập hoàn chỉnh với phân tách Public/Private rõ ràng.
* Áp dụng Terraform để quản lý hạ tầng dưới dạng code (Infrastructure as Code).
* Các dịch vụ nền tảng như ECR, ECS và ALB đã sẵn sàng cho việc triển khai ứng dụng.

---

### Khó khăn & Bài học kinh nghiệm

* **Khó khăn:** Thiết kế VPC và cấu hình routing ban đầu khá phức tạp.
* **Giải pháp:** Làm theo best practices của AWS và kiểm tra từng bước.
* **Bài học:** Thiết kế hạ tầng tốt ngay từ đầu giúp giảm rất nhiều vấn đề về mở rộng và bảo trì sau này.

---

### Kế hoạch tuần tiếp theo

* Triển khai backend lên ECS Fargate.
* Tích hợp xác thực người dùng với Amazon Cognito.
* Kết nối frontend với backend API.
