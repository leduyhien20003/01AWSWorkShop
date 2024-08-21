---
title : "MỞ RỘNG THÊM CHỨC NĂNG"
date :  "`r Sys.Date()`" 
weight : 5 
chapter : false
pre : " <b> 2.5. </b> "
---

{{% notice info %}}
Để hoàn thiện bước này các bạn cần có kiến thức cơ bản về Javascript, Python.
{{% /notice %}}

Sau khi hoàn thành phần **Route53** các bạn đã sở hữu cho mình một website sơ yếu lý lịch hoàn chỉnh cho riêng mình, các bạn có thể dùng nó để thêm vào CV xin việc. Nhưng để có thể gây ấn tượng hơn về khả năng sử dụng các dịch vụ AWS của bản thân với nhà tuyển dụng, mình sẽ hướng dẫn các bạn thêm vào một chức năng nho nhỏ đó là hiển thị số lượt xem trang. 
{{% notice note %}}
Đây là phần mở rộng thêm, các bạn có thể bỏ qua. 
{{% /notice %}}

Trong phần này chúng ta sẽ sử dụng các dịch vụ sau:
- Lambda function
- API Gateway
- DynamoDB

**Sơ bộ toàn bộ hệ thống của chúng ta như sau**
![ConnectPrivate](01AWSWorkShop/images/s3-satic-basic.jpg)

**Các bước thực hiện**
1. [Tạo database lưu trữ số lượt xem](2.5.1-Dynamodb/)

2. [Tạo một Lambda function để cập nhật số lượt xem](2.5.2-Lambda/)

3. [Tạo API kết nối với database](2.5.3-APIgateway/)

4. [Tạo hiển thị số lượt xem lên trang web](2.5.4-Javascript/)