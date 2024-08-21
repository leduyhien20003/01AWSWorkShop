---
title : "TRỎ DOMAIN NAME TỚI CLOUDFRONT"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.4.2 </b> "
---

**Trước khi có thể trỏ domain name tới **CloudFront** chúng cần phát hành cho nó một certificate**

**1**. Truy cập vào dịch vụ **AWS Certificate Manager**, tại giao diện chính chọn **Request a certificate**
       ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront1.jpg)

**2**. **Certificate type** để là **Request a public certificate**, rồi chọn **Next**
       ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront2.jpg)

**3**. Điền **Domain names** của mình vào rồi còn lại để mặc định, cuộn xuống chọn **Request**
       ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront3.jpg)

**4**. Chọn **List certificates**, sau đó chọn certificate vừa tạo, kéo xuống phần **Domains**, chọn **Create records in Route 53**
      ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront4.jpg)
 - Sau đó các bạn chọn **Create records**
  ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront5.jpg)

{{% notice info %}}
Cách này dùng cho các bạn dùng domain của **Route53**, với các nhà cung cấp khác, các bạn có thể tìm kiếm trên mạng cách phát hành certificate nha
{{% /notice %}}  
  
**5**. Các bạn đợi vài phút, bao giờ **Status** chuyển thành **Issued** như thế này là phát hành thành công nha 
 ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront6.jpg)

**6**. Bây giờ quay lại giao diện **Route53**, chọn **Hosted zones**, nhấn vào domain của mình
 ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront7.jpg)

**7**. Chọn **Records**, chọn **Create record**
 ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront8.jpg)

- Trong giao diện **Create record**, các bạn điền như sau
![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront9.jpg)

**8**. Bây giờ các bạn quay lại **CloudFront**, chọn **Distribution** ta đang sử dụng
- Trong phần **General**, tại phần **Settings**, chọn **Edit**
  ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront10.jpg)

**9**. Trong giao diện **Edit**, tại mục **Alternate domain name (CNAME)** điền như thế này ạ, rồi chọn **Save Changes** 
 ![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront11.jpg)
 
{{% notice info %}}
Trong phần phát hành certificate, mình quên mất là **CloudFront** chỉ chấp nhận certificate ở **US East (N. Virginia) Region (us-east-1)**, các bạn nào phát hành ở regiion khác chịu khó làm lại phần phát hành certificate 😁
{{% /notice %}}  

**10**. Các bạn đợi một lúc cho **CloudFront** deploy xong rồi các bạn truy cập bằng domain name của mình để kiểm tra kết nối
![ConnectPrivate](01AWSWorkShop/images/DNSCloudFront12.jpg)
**Thành Công !!**