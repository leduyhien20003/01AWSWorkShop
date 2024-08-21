---
title : "KIỂM TRA CLOUDFRONT"
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 2.3.3 </b> "
---

**Trong giao diện CloudFront distribution**

- Ở phần **Distribution**, chọn distribution vừa tạo
![ConnectPrivate](01AWSWorkShop/images/check-cloufront1.jpg)

- Đảm bảo rằng CloudFront đã deploy xong bằng cách xem nội dung ở mục **Last modified**
![ConnectPrivate](01AWSWorkShop/images/check-cloufront2.jpg)

- Sao chép **Distribution domain name**, dán vào trình duyệt và kiểm tra xem ta có kết nối đến trang web được hay không
![ConnectPrivate](01AWSWorkShop/images/check-cloufront3.jpg)

**Thành công rồi!**  

Đến bước này là ta đã thành công có cho bản thân một trang web sơ yếu lý lịch, nhưng cái DNS của Cloudfront khá là xấu và chưa làm rõ được tính cá nhân của trang sơ yếu lý lịch, để khắc phục vấn đề này ta chuyển đến bước tiếp theo nha.

