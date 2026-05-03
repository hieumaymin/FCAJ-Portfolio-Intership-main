---
title: "Worklog Tuần 5"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5

* Triển khai cơ sở dữ liệu trên AWS.
* Bảo mật thông tin nhạy cảm của hệ thống.
* Cấu hình HTTPS và domain riêng cho ứng dụng.

---

### Công việc đã thực hiện trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|------|-----------|--------------|---------------|---------------------|
| 1 | - Khởi tạo Amazon RDS (PostgreSQL) <br>&emsp; + Triển khai trong Private Subnet <br>&emsp; + Cấu hình instance phù hợp | 06/04/2026 | 06/04/2026 | [RDS in VPC Guide](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.WorkingWithRDSInstanceInVPC.html), [DB Subnet Groups](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.WorkingWithRDSInstanceInVPC.html#USER_VPC.SubnetGroups) |
| 2 | - Migration database <br>&emsp; + Kết nối ECS Service với RDS <br>&emsp; + Triển khai schema database | 07/04/2026 | 07/04/2026 | [ECS to RDS Connectivity](https://aws.amazon.com/premiumsupport/knowledge-center/ecs-tasks-container-rds-database/), [TypeORM Migration Guide](https://typeorm.io/migrations) |
| 3 | - Thiết lập AWS Secrets Manager <br>&emsp; + Lưu trữ thông tin database an toàn <br>&emsp; + Loại bỏ thông tin hardcode trong code | 08/04/2026 | 08/04/2026 | [Secrets Manager Best Practices](https://docs.aws.amazon.com/secretsmanager/latest/userguide/best-practices.html), [ECS Secrets Injection](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/specifying-sensitive-data-tutorial.html) |
| 4 | - Cấu hình VPC Endpoint <br>&emsp; + Gateway Endpoint cho S3 <br>&emsp; + Tối ưu truy cập nội bộ | 09/04/2026 | 09/04/2026 | [S3 Gateway Endpoints](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints-s3.html), [Gateway vs Interface Endpoints](https://docs.aws.amazon.com/vpc/latest/privatelink/gateway-endpoints.html) |
| 5 | - Cấu hình HTTPS <br>&emsp; + Tạo SSL Certificate bằng ACM <br>&emsp; + Gắn certificate vào ALB | 10/04/2026 | 10/04/2026 | [AWS Certificate Manager Guide](https://docs.aws.amazon.com/acm/latest/userguide/acm-overview.html), [ALB HTTPS Listeners](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/create-https-listener.html) |
| 6 | - Cấu hình domain riêng <br>&emsp; + Mapping domain bằng Route 53 <br>&emsp; + Kết nối với ALB và Amplify | 11/04/2026 | 11/04/2026 | [Route 53 Alias Records](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-choosing-alias-non-alias.html), [Amplify Custom Domains](https://docs.aws.amazon.com/amplify/latest/userguide/custom-domains.html) |
| 7 | - Kiểm tra bảo mật hệ thống <br>&emsp; + Đóng các port không cần thiết <br>&emsp; + Rà soát lại Security Group | 12/04/2026 | 12/04/2026 | - |

---

### Kết quả đạt được

* Database hoạt động ổn định trong môi trường private network.
* Thông tin nhạy cảm được quản lý an toàn bằng Secrets Manager.
* Hệ thống đã hỗ trợ HTTPS và domain riêng.

---

### Khó khăn & Bài học kinh nghiệm

* **Khó khăn:** Quản lý kết nối giữa ECS và RDS để tránh quá tải database.
* **Giải pháp:** Theo dõi số lượng connection và kiểm soát quá trình migration hợp lý.
* **Bài học:** Bảo mật cần được triển khai ngay từ đầu, không nên để đến giai đoạn sau.

---

### Kế hoạch tuần tiếp theo

* Thiết lập monitoring hệ thống bằng CloudWatch.
* Thực hiện kiểm thử hiệu năng.
* Cấu hình theo dõi chi phí và cảnh báo.