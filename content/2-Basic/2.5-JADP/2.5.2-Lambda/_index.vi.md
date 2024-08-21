---
title : "TẠO LAMBDA FUNCTION"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.5.2 </b> "
---

Trong phần này chúng ta sẽ tạo một Lambda function để có thể lấy số lượt xen cũng như cập nhật lại số lượt xem với Dynamodb.

### Giới thiệu

**Lambda** là một service serverless của AWS cho phép người dùng thực thi code mà không cần quan tâm tới hạ tầng phía sau

### Tạo Lambda function

- Trong giao diện **Lambda**, chọn **Create function**
![ConnectPrivate](01AWSWorkShop/images/Lambda1.jpg)
- Trong giao diện **Create function**, chọn **Author from scratch**, điền **Function name**, còn **Runtime** chọn ngôn ngữ các bạn dùng viết code, phần còn lại để mặc định, chọn **Create function**
![ConnectPrivate](01AWSWorkShop/images/Lambda2.jpg)
- Sau khi tạo **Lambda function** thành công, các bạn chọn function vừa tạo, chọn **Configuration** 

  Trong **Execution role**, click vào đường link bên dưới **Role name**
  ![ConnectPrivate](01AWSWorkShop/images/Lambda3.jpg)
- Trong giao diện **IAM Roles** của function chọn **Add permissions**, **Attach policies**
  ![ConnectPrivate](01AWSWorkShop/images/Lambda4.jpg)
  Chọn **AmazonDynamoDBFullAccess**, rồi chọn **Add permissions**
  ![ConnectPrivate](01AWSWorkShop/images/Lambda5.jpg)
- Quay lại giao diện của Lambda function, chọn **Code**, dán code đã chuẩn bị vào và nhấn **Deploy**(bên dưới là code của mình các bạn có thể tham khảo)
  ![ConnectPrivate](01AWSWorkShop/images/Lambda6.jpg)
Vậy là ta đã tạo xong **Lambda function**, ta sang bước tiếp theo