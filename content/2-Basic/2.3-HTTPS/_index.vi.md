---
title : "BẢO MẬT VÀ TĂNG TỐC"
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 2.3. </b> "
---

### Tăng tốc và bảo mật kết nối đến Static Website với Cloudfront

 Sau khi hoàn thành bước trước, chúng ta đã host một trang web sơ yếu lý lịch tĩnh thành công bằng dịch vụ **Amazon S3**, nhưng cần phải public S3 của mình, một điều có thể dẫn đến các vấn đề bảo mật nghiêm trọng! Rất may mắn là AWS có một dịch vụ có thể giúp chúng ta khắc phục vấn đề này, đó chính là **Amazon CloudFront**.
 
### Giới thiệu
 CloudFront là một CDN service của AWS, viết tắt của Content Delivery Network, một mạng lưới giúp delivery nội dung tới người dùng cuối một cách nhanh chóng và bảo mật nhờ vào việc điều hướng request của họ tới các máy chủ chứa tài nguyên gần nhất, hỗ trợ nhiều tính năng bảo mật, bao gồm kết nối HTTPS, chữ ký số (Certificate) và xác thực người dùng.


**Các bước thực hiện**

1. [Chặn tất cả truy cập công cộng vào S3](2.3.1-BlockPublic/)

2. [Tạo và cấu hình Amazon CloudFront](2.3.2-CreateCF/)

3. [Kiểm tra CloudFront](2.3.3-CheckCF/)