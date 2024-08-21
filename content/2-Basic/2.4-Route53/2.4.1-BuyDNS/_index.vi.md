---
title : "MUA DOMAIN NAME VỚI ROUTE53"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 2.4.1 </b> "
---

**1**. Chúng ta truy cập vào giao diện **Route53**, các bạn kéo xuống phần **Register domain** 

- Trong phần **Register domain**, các bạn điền tên domain mong muốn kiểm tra, nếu có **Exact match** là được nha, các bạn  chọn **Select**, rồi **Proceed to checkout**
  ![ConnectPrivate](/01AWSWorkShop/images/BuyDNS1.png)
  ![ConnectPrivate](/01AWSWorkShop/images/BuyDNS2.png)
{{% notice tip %}}
Các bạn nên chọn đuôi **.click** vì theo mình tìm hiểu thì đuôi này rẻ nhất rồi, giá 3 dollar.
{{% /notice %}}

**2**. Tới đây các bạn có thể chọn **Auto-renew** hoặc không ở dây mình không chọn, rồi chuyển qua bước tiếp theo
![ConnectPrivate](/01AWSWorkShop/images/BuyDNS3.png)
**3**. Trong phần **Registrant contact** các bạn điền các thông tin cá nhân của mình rồi chuyển đến bước tiếp theo thôi
![ConnectPrivate](/01AWSWorkShop/images/BuyDNS4.png)
**4**. Các bạn kiểm tra lại các thông tin của mình lần cuối, đồng ý với **Terms and conditions**, rồi chọn **Submit**. 
![ConnectPrivate](/01AWSWorkShop/images/BuyDNS5.png)
- **Lưu ý**:  sau đó họ sẽ gửi cho các bạn email yêu cầu xác thực email đăng ký domain, các bạn bấm vào đường link xác thực là xong
![ConnectPrivate](/01AWSWorkShop/images/BuyDNS7.png)

Tới đây các bạn chọn **Requests** ở phần **Domains** tại bảng bên trái để xem yêu cầu mình vừa thực hiện. Các bạn đợi một lúc, bao giờ phần **Status** chuyển thành **Successful** là chúng ta đã mua domain thành công rồi nha.
![ConnectPrivate](/01AWSWorkShop/images/BuyDNS6.png)
{{% notice warning %}}
Nếu bạn nào **Request** bị **Failed** thì mời các bạn xem phần khắc phục lỗi khi mua domain name!! 
{{% /notice %}}