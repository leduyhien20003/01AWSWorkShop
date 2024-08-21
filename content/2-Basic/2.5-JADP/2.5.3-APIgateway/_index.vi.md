---
title : "TẠO API GATEWAY"
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 2.5.3 </b> "
---


Chúng ta không nên kết nối trực tiếp từ code của mình đến **DynamoDB**, mà nên qua một bước trung gian đó là **API Gateway** (lý do thì nhiều vô kể, các bạn có thể tìm kiếm thêm trên mạng nha), ở đây ta sử dụng dịch vụ **API Gateway** của AWS.

### Giới thiệu

**API Gateway** là một dịch vụ API Gateway được cung cấp bởi AWS. Nó cung cấp 
một cách đơn giản để xây dựng, quản lý và bảo mật các RESTful API hoặc WebSocket. AWS API Gateway là một dịch vụ quan trọng trong kiến trúc dựa trên các dịch vụ của AWS (AWS-based microservices architecture) và thường được sử dụng cùng với các dịch vụ AWS khác như AWS Lambda, EC2, S3, Amazon DynamoDB.
API Gateway là một service chủ yếu có nhiệm vụ nhận request của client sau đó forward tới các service phía sau.

### Tạo API Gateway 

- Trong giao diện **API Gateway**, ta chọn **Create API**
![ConnectPrivate](/01AWSWorkShop/images/API1.jpg)

- Trong giao diện **Create API**, ở phần **REST API** ta chọn **Build**
![ConnectPrivate](/01AWSWorkShop/images/API2.jpg)

- Tiếp theo chọn **New API**, đặt tên cho API, còn lại để mặc định rồi chọn **Create API**
![ConnectPrivate](/01AWSWorkShop/images/API3.jpg)

- Ta chọn API vừa tạo, rồi chọn **Create resource**, nhập **Resource path**, chọn **Create resource**
![ConnectPrivate](/01AWSWorkShop/images/API4.jpg)
![ConnectPrivate](/01AWSWorkShop/images/API5.jpg)

- Cũng trong giao diện API vừa tạo, ta chọn **Create method**
  ![ConnectPrivate](/01AWSWorkShop/images/API6.jpg)

  Bên trong giao diện **Create method**, **Method type** chọn **GET**(ta cần hai type là **GET** và **POST**, làm tương tự nhau), **Integration type** để nguyên, **Lambda function** chọn cái ta vừa tạo ở bước trước, chọn **Create method** để hoàn thành
  ![ConnectPrivate](/01AWSWorkShop/images/API7.jpg)

Đến đây gần như là thành công rồi, nhưng ta vẫn cần làm thêm 1 bước nữa, ta quay lại giao diện **Lambda function** đã tạo ở bước trước chọn **Configuration**, chọn **Permissions** ở cột bên trái.

- Cuộn xuống phần **Resource-based policy statements**, chọn **Add permissions**

  Trong giao diện **Add permissions**, chọn **AWS service**, rồi điền như dưới đây(làm tương tự cho phương thức **GET**), rồi chọn **Save**
  ![ConnectPrivate](/01AWSWorkShop/images/API8.jpg)

Tới đây là hoàn thành rồi, ta quay lại giao diện của **API Gateway**, chọn **Deploy API**

- Trong giao diện **Deploy API**, phần **Stage** chọn New stage, tên đặt tùy ý, và chọn **Deploy**
  ![ConnectPrivate](/01AWSWorkShop/images/API9.jpg)
- Ta sang phần **Stages**, copy **Invoke URL** để dùng cho bước sau
  ![ConnectPrivate](/01AWSWorkShop/images/API10.jpg)
  
Vậy là ta hoàn thành 3/4 công việc rồi, mời các bạn sang bước tiếp theo!
