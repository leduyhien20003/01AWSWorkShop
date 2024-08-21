---
title : "Giới thiệu chung"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

![ConnectPrivate](01AWSWorkShop/images/icons3.png)

S3, viết tắt của **Simple Storage Service**
là một dịch vụ lưu trữ dạng Object cung cấp khả năng mở rộng, 
availability, performance. 
Người dùng có thể sử dụng S3 để lưu trữ và bảo vệ nhiều loại data cho các 
usecase như: data lake, website, mobile, backup & restore, 
archive, enterprise application, IoT device, Big Data & Analytic. 
S3 cung cấp nhiều managed feature giúp tối ưu, tổ chức và cấu 
hình access tới data đáp ứng nhu cầu về business, organization & 
complicance.

**Đặc trưng cơ bản của S3**
-  Là một Managed Service. User không cần quan tâm tới hạ tầng ở bên dưới.
-  Cho phép lưu file dưới dạng object với size từ 0 - 5TB
-  High Durability (11 9s), Scalability, High Availability (99.99%), High performance.
-  Usecase đa dạng (mọi bài toán về lưu trữ từ lớn tới nhỏ đều có thể sd S3).
-  Cung cấp nhiều class lưu trữ để tiết kiệm chi phí cho từng loại data.
-  Cung cấp khả năng phân quyền và giới hạn truy cập một cách chi tiết.
-  Dễ sử dụng, có thể kết hợp với nhiều service khác cho bài toán automation và 
data processing.

**S3 Static Website Hosting**
- S3 có hỗ trợ người dùng host 1 website tĩnh (chỉ bao gồm html, css, js, image...)
- Được thừa hưởng toàn bộ đặc tính của S3 (Durability, HA)
- Không cần duy trì server, giảm effort Administration.
- Hỗ trợ setting CORS nhằm tránh tài nguyên bị khai thác bởi website khác.
- Kết hợp với dịch vụ CDN (CloudFront) có thể giúp tăng tốc độ truy cập khi user 
nằm ở các region khác nhau.

**Hầu hết các framework frontend hiện nay như Angular, Vue, NodeJS đều hỗ trợ build ra 1 website tĩnh để có thể deploy lên S3 sau khi code xong**
