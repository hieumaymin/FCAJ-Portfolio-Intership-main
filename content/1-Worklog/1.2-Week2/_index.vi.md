---
title: "Worklog Tuần 2"
date: "2026-03-09"
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2

* Học và thực hành các dịch vụ Compute của AWS (EC2, AMI, EBS, Auto Scaling, ELB).
* Nâng cao kỹ năng giám sát và sao lưu với CloudWatch và AWS Backup.
* Tìm hiểu các dịch vụ lưu trữ của AWS (S3, Storage Gateway, FSx).
* Thực hành triển khai, mở rộng hệ thống và host website tĩnh.

---

### Công việc đã thực hiện trong tuần

| Ngày | Công việc | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|------|-----------|--------------|---------------|---------------------|
| 1 | - Tìm hiểu AWS Compute & EC2 <br>&emsp; + Kiến trúc EC2, loại instance, mô hình giá (On-demand, Spot, Reserved) <br>&emsp; + AMI, Snapshot, EBS và Instance Store <br>&emsp; + Khởi tạo EC2 (Linux & Windows) <br>&emsp; + Kết nối bằng SSH và RDP <br>&emsp; + Deploy ứng dụng Node.js CRUD trên EC2 | 16/03/2026 | 16/03/2026 | [EC2 User Guide](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html), [EBS vs Instance Store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html) |
| 2 | - Khả năng mở rộng và giám sát <br>&emsp; + Cấu hình Auto Scaling Group <br>&emsp; + Thiết lập Elastic Load Balancer (ELB) <br>&emsp; + Giám sát bằng CloudWatch (metrics, logs, alarms) <br>&emsp; + Cấu hình AWS Backup cho EC2 và các dịch vụ liên quan | 17/03/2026 | 17/03/2026 | [Auto Scaling Guide](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html), [CloudWatch Logs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html) |
| 3 | - Tìm hiểu Amazon S3 <br>&emsp; + Kiến trúc lưu trữ object <br>&emsp; + Các lớp lưu trữ (Standard, IA, Glacier) <br>&emsp; + Cấu hình Bucket Policy, ACL, Versioning <br>&emsp; + Lifecycle và lưu trữ dài hạn | 18/03/2026 | 18/03/2026 | [S3 Storage Classes](https://aws.amazon.com/s3/storage-classes/), [S3 Lifecycle Management](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html) |
| 4 | - Lưu trữ Hybrid với Storage Gateway <br>&emsp; + Tổng quan hybrid cloud storage <br>&emsp; + Triển khai File Gateway trên EC2 <br>&emsp; + Cấu hình NFS File Share liên kết S3 <br>&emsp; + Mount storage từ máy local | 19/03/2026 | 19/03/2026 | [Storage Gateway Guide](https://docs.aws.amazon.com/storagegateway/latest/userguide/WhatIsStorageGateway.html), [File Gateway Setup](https://docs.aws.amazon.com/storagegateway/latest/userguide/CreatingAnS3FileGateway.html) |
| 5 | - Lưu trữ quản lý & hosting <br>&emsp; + Triển khai Amazon FSx for Windows File Server <br>&emsp; + Cấu hình chia sẻ file (SMB) <br>&emsp; + Host website tĩnh bằng S3 <br>&emsp; + Cấu hình CloudFront và OAI để tăng bảo mật và hiệu năng | 20/03/2026 | 20/03/2026 | [Amazon FSx Guide](https://docs.aws.amazon.com/fsx/latest/WindowsGuide/what-is.html), [CloudFront OAC/OAI](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html) |
| 6 | - Ôn tập và thực hành <br>&emsp; + Ôn lại EC2, S3, Auto Scaling <br>&emsp; + Làm thêm các lab triển khai | 21/03/2026 | 21/03/2026 | [AWS Architecture Center](https://aws.amazon.com/architecture/), [AWS Self-Paced Labs](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/) |
| 7 | - Kiểm tra và tổng kết <br>&emsp; + Test Auto Scaling và Load Balancing <br>&emsp; + Kiểm tra hệ thống monitoring và backup <br>&emsp; + Tổng hợp kiến thức và chuẩn bị tuần tiếp theo | 22/03/2026 | 22/03/2026 | - |

---

### Kết quả đạt được

* Hiểu rõ EC2, AMI, EBS và cách triển khai instance.
* Triển khai thành công EC2 Linux và Windows.
* Thiết lập Auto Scaling và Elastic Load Balancer để đảm bảo tính sẵn sàng cao.
* Giám sát hệ thống bằng CloudWatch (metrics, logs, alarms).
* Cấu hình AWS Backup để tự động sao lưu dữ liệu.
* Nắm vững Amazon S3 (storage class, lifecycle, phân quyền).
* Triển khai static website hosting với S3 và CloudFront.
* Tìm hiểu lưu trữ hybrid (Storage Gateway) và hệ thống file FSx.

---

### Khó khăn & Bài học kinh nghiệm

* **Khó khăn:** Khó nắm bắt cách các dịch vụ AWS kết hợp với nhau.
* **Giải pháp:** Thực hành lab nhiều và học theo mô hình kiến trúc chuẩn.
* **Bài học:** Sự kết hợp giữa compute, storage và monitoring là yếu tố quan trọng để xây dựng hệ thống cloud ổn định.

---

### Kế hoạch tuần tiếp theo

* Chốt yêu cầu chức năng và các tiêu chuẩn phi chức năng (NFR) cho ứng dụng Spendwise.
* Khởi tạo chiến lược quản lý hạ tầng bằng Terraform (S3 backend/State strategy).


