---
title : "Xây dựng resume website"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2. </b> "
---

{{% notice info %}}
Bạn cần tạo sẵn 1 S3 bucket để thực hiện bài thực hành này.
{{% /notice %}}

Trong phần này chúng ta sẽ dựng một website sơ yếu lý lịch tĩnh đơn giản bằng các dịch vụ sau:
- Route 53
- Cloudfront
- S3 bucket
- Certificate Manager
- Lambda function
- API Gateway
- Dynamo DB

![ConnectPrivate](/01AWSWorkShop/images/s3-satic-basic.jpg)

### Nội dung
  - [HTML, CSS](2.1-HTML,CSS/)
  - [Bật tính năng static website](2.2-StaticWeb/)
  - [Bảo mật và tăng tốc truy cập](2.3-HTTPS/)
  - [DNS](2.4-Route53/)
  - [Mở rộng thêm chức năng](2.5-JADP/)
  - [Kết quả](2.6-Result/)
