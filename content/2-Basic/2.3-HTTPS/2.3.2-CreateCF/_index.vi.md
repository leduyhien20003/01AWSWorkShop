---
title : "TẠO VÀ CẤU HÌNH CLOUDFRONT"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.3.2 </b> "
---

**Trong giao diện CloudFront distribution**

- Chọn **Create a CloudFront distribution**
![ConnectPrivate](/01AWSWorkShop/images/cloufront1.jpg)

- Trong phần **Origin domain**, chọn bucket chứa trang web sơ yếu lý lịch của bản thân
  
  Phần **Origin path** các bạn không điền cũng được
![ConnectPrivate](/01AWSWorkShop/images/cloufront2.jpg)

- Trong phần **Origin access**, chúng ta chọn **Origin access control settings**, nếu các bạn đã có **Origin access control** rồi thì dùng nếu không ta chọn **Create new OAC** ở bên cạnh.
![ConnectPrivate](/01AWSWorkShop/images/cloufront3.jpg)
 
  Trong cửa sổ **Create new OAC** các bạn để mặc định, có thể điền **Description** hoặc không, sau đó các bạn chọn **Create** rồi copy OAC vừa tạo lưu vào đâu đó, ta sẽ dùng OAC này sau.
  ![ConnectPrivate](/01AWSWorkShop/images/cloufront4.jpg)

- Trong phần **Viewer**, ở mục **Viewer protocol policy** các bạn chọn **Redirect HTTP to HTTPS**
![ConnectPrivate](/01AWSWorkShop/images/cloufront5.jpg)

- Trong phần **Web Application Firewall (WAF)**, các bạn chọn **Do not enable security protections**
 
  Các phần còn lại các bạn để mặc định
  
  Cuộn xuống dưới chọn **Create distribution**, các bạn đợi vài phút là **Distribution** sẵn sàng để sử dụng
![ConnectPrivate](/01AWSWorkShop/images/cloufront6.jpg)
- Trong lúc đợi **Distribution** sẵn sàng, các bạn có nhớ cái OAC mình tạo trước đó không, giờ ta sẽ sử dụng nó để thay đổi **S3 Bucket policy**. Tại sao ta phải làm thế, do ở bước **Chặn truy cập công cộng vào s3** tất cả truy cập công cộng đã bị chặn bao gồm cả Cloudfront, cái OAC ta tạo dùng để S3 cho phép **Distribution** của ta kết nối đến Bucket chứa website của mình.

  Trong giao diện **S3 bucket**, chọn **Permissions**, kéo xuống phần **Bucket policy** chọn **Edit**, dán OAC ta tạo trước đó vào rồi lưu là xong, giờ đây **Distribution** của ta đã kết nối được đến S3. 
  ![ConnectPrivate](/01AWSWorkShop/images/cloufront7.jpg)
