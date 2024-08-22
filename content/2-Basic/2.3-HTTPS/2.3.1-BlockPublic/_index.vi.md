---
title : "CHẶN TRUY CẬP CÔNG CỘNG VÀO S3"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 2.3.1 </b> "
---

**1**. Trong giao diện **S3 bucket**

- Chọn **Permissions**
- Hiện tại, chức năng **Block all public access** đang Off do chúng ta đã bật tắt tại bước **Bật tính năng static website**
- Chọn **Edit**
![ConnectPrivate](/01AWSWorkShop/images/S3-public-access4.jpg)

- Chọn **Block all public access**
- Chọn **Save changes**
![ConnectPrivate](/01AWSWorkShop/images/s3-blockpublic1.jpg)

- Chọn **confirm** trong cửa sổ **Confirm**
![ConnectPrivate](/01AWSWorkShop/images/s3-blockpublic2.jpg)
- **Block all public access** đã được bật, lúc này sẽ không có bất kỳ một truy cập công cộng nào có thể kết nối được với S3 Bucket của bạn
![ConnectPrivate](/01AWSWorkShop/images/s3-blockpublic3.jpg)
- Cuộn xuống **Bucket policy**, chọn **Delete**

**2**. Kiểm tra chức năng **Block all public access**

- Cuộn xuống cuối trang, tại mục **Static website hosting**
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening4.jpg)
- Chọn ký hiệu ô vuông để copy **URL**, dán **URL** vừa copy vào trình duyệt để kiểm tra
![ConnectPrivate](/01AWSWorkShop/images/s3-blockpublic4.jpg)

Đến đây chúng ta đã **Block all public access** thành công
