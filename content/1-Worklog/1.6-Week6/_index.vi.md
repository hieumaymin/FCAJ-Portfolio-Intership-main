---
title: "Worklog Tuần 6"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục Tiêu Tuần 6

* Triển khai **AWS WAF** bảo vệ ứng dụng khỏi các lỗ hổng web phổ biến.
* Thiết lập **Bastion Host** (EC2) để truy cập quản trị DB an toàn từ xa.
* Tự động hóa đồng bộ dữ liệu người dùng thông qua AWS Lambda.

### Các công việc thực hiện trong tuần

| Ngày | Công việc | Bắt đầu | Hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - Khởi tạo AWS WAF Web ACL và gắn vào ALB của hệ thống | 13/04/2026 | 13/04/2026 | [AWS WAF Developer Guide](https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html), [Associating WAF with ALB](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-associating-aws-resource.html) |
| 2 | - Cấu hình WAF Rules cho SQLi, XSS và giới hạn Rate Limit | 14/04/2026 | 14/04/2026 | [AWS Managed Rules for WAF](https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-list.html), [WAF Rate-based Rules](https://docs.aws.amazon.com/waf/latest/developerguide/waf-rule-statement-type-rate-based.html) |
| 3 | - Triển khai EC2 Bastion host nhỏ phục vụ port forwarding tới DB | 15/04/2026 | 15/04/2026 | [Linux Bastion Hosts on AWS](https://aws.amazon.com/quickstart/architecture/linux-bastion/), [Securely Connect to Private DB](https://aws.amazon.com/blogs/database/securely-connect-to-an-amazon-rds-postgresql-database-instance-from-outside-a-vpc/) |
| 4 | - Triển khai **AWS Lambda** (PostConfirmation) để đồng bộ Cognito-RDS | 16/04/2026 | 16/04/2026 | [Cognito Post Confirmation Trigger](https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-lambda-post-confirmation.html), [Lambda with RDS Proxy](https://aws.amazon.com/blogs/compute/using-amazon-rds-proxy-with-aws-lambda/) |
| 5 | - Kiểm toán bảo mật Bastion và giới hạn dải IP truy cập | 17/04/2026 | 17/04/2026 | [Security Group Best Practices](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html), [AWS IAM Policies for EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-policies-for-amazon-ec2.html) |
| 6 | - Kiểm thử đăng ký người dùng mới và verify tính nhất quán dữ liệu | 18/04/2026 | 18/04/2026 | [Testing Lambda Triggers](https://docs.aws.amazon.com/lambda/latest/dg/testing-guide.html), [Amazon RDS Data Consistency](https://aws.amazon.com/rds/features/consistency/) |
| 7 | - Review log truy cập WAF và hiệu quả chặn request độc hại | 19/04/2026 | 19/04/2026 | - |

### Kết quả đạt được Tuần 6

* Tăng cường bảo mật API bằng cách chặn các request độc hại thông qua WAF.
* Thiết lập đường dẫn quản trị DB an toàn mà không cần công khai RDS ra Internet.
* Tự động hóa 100% quy trình đồng bộ hồ sơ người dùng qua Lambda.

### Kế hoạch Tuần tới

* Tinh chỉnh chính sách Auto-scaling cho ECS Fargate.
* Phân tích sâu dữ liệu logs bằng CloudWatch Logs Insights.