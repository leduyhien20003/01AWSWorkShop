---
title : "TẠO CHỨC NĂNG HIỂN THỊ LƯỢT XEM"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 2.5.4 </b> "
---

Tại bước này ta sẽ dùng ngôn ngữ JavaScript viết một chức năng nho nhỏ để hiện thị số lượt xem, code này sẽ call đến API, rồi API sẽ call đến các dịch vụ sau.

- **Dưới đây là code của mình các bạn có thể tham khảo**

![ConnectPrivate](01AWSWorkShop/images/JS1.jpg)

- Sau đó các bạn upload lại file web sơ yếu lý lịch của mình lên lại **S3**
 
  Các bạn đợi một khoảng thời gian cho **CloudFront** cập nhật lại hoặc các bạn cũng có thể làm cách sau để cập nhật luôn
  - Các bạn truy cập vào **CloudFront**, sau đó chọn **Distribution** chúng ta đang sử dụng, chọn **Invalidations** và chọn **Create invalidation**
  ![ConnectPrivate](01AWSWorkShop/images/JS2.jpg)

  - Trong giao diện **Create invalidation**, các bạn cập nhật file nào thì điền đường dẫn file đó, không nên **(/*)** sẽ tốn nhiều chi phí nếu ta có nhiều file.

Sau khi hoàn thành bước này các đã hoàn thành phần 1!