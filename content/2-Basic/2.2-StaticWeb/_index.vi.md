---
title : "BẬT WEBSITE HOSTING"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.2. </b> "
---

### Bật tính năng static website

**1**. Tiếp theo, chúng ta sẽ bật tính năng Static website.

- Trong giao diện S3 bucket, chọn **Properties**.
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening1.jpg)

**2**. Trong giao diện **Properties**:

- Kéo xuống và chọn Edit trong mục Static website hosting.
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening2.jpg)

**3**. Trong giao diện **Static website hosting**:

- Chọn Enable cho Static website hosting.
- Ở mục Hosting type, chọn Host a static website.
- Ở mục Index document, nhập **index.html**.
- Ở mục Error document, nhập **error.html**.
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening3.jpg)

**4**. Kiểm tra lại thông tin và chọn **Save changes**.

**5**. Hoàn thành việc bật tính năng **Static website hosting**.
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening4.jpg)

**Để truy cập vào website được host, chúng ta cần cấu hình lại Block Public Access như sau:**

**6**. Trong giao diện **S3 bucket**:

- Chọn Permissions.
- Lúc này, bạn sẽ thấy Block all public access đang ở trạng thái On.
![ConnectPrivate](/01AWSWorkShop/images/S3-public-access1.jpg)

**7**. Trong giao diện **Block public access**:

- Bỏ chọn Block all public access.
- Chọn Save changes.
![ConnectPrivate](/01AWSWorkShop/images/S3-public-access2.jpg)

**8**. Xác nhận bằng cách chọn Confirm trong hộp thoại confirm
![ConnectPrivate](/01AWSWorkShop/images/S3-public-access3.jpg)

**9**. Hoàn thành cấu hình **Block Public Access**
![ConnectPrivate](/01AWSWorkShop/images/S3-public-access4.jpg)

**Đến đây gần như là thành công rồi, chúng ta vẫn cần cấu hình lại Bucket policy cho phép mọi người access:**

**10**. Trong giao diện **S3 bucket**:

- Chọn Permissions.
- Lúc này, bạn sẽ thấy Bucket policy, ta chọn **Edit**.
![ConnectPrivate](/01AWSWorkShop/images/S3-bucket-policy1.jpg)

**11**. Trong giao diện **Edit bucket policy**:
- Chọn **Policy generator**. 
![ConnectPrivate](/01AWSWorkShop/images/S3-bucket-policy2.jpg)

**12**. Trong giao diện **Policy generator**:
- Ta tạo một policy cho phép mọi người access, sau đó copy rồi dán vào phần **Policy** trong giao diện **Edit bucket policy** và chọn **Save changes**.
![ConnectPrivate](/01AWSWorkShop/images/S3-bucket-policy3.jpg)
![ConnectPrivate](/01AWSWorkShop/images/S3-bucket-policy4.jpg)
![ConnectPrivate](/01AWSWorkShop/images/S3-bucket-policy5.jpg)
Vậy là ta đã có thể truy cập vào trang sơ yếu lý lịch của bản thân bằng đường link dưới đây
![ConnectPrivate](/01AWSWorkShop/images/S3-static-opening4.jpg)