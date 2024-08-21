---
title : "TẠO DATABASE"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 2.5.1 </b> "
---


Trước khi có thể hiển thị số lượt xem lên trang web, chúng ta cần có một nơi để lưu trữ nó, ở đây vì ta đang làm về các dịch vụ của AWS nên mình sẽ hướng dẫn các bạn sử dụng **DynamoDB** để tạo cơ sở dữ liệu lưu trữ.

### Giới thiệu

**Amazon DynamoDB** là một cơ sở dữ liệu NoSQL dạng key-value, hoàn toàn có thể quản lý và không cần máy chủ, được thiết kế để chạy các ứng dụng hiệu suất cao ở bất kỳ quy mô nào. DynamoDB cung cấp các tính năng bảo mật tích hợp, sao lưu liên tục, sao chép tự động nhiều khu vực, bộ nhớ đệm trong bộ nhớ, và các công cụ nhập xuất dữ liệu.

{{% notice note %}}
Về NoSQL, các có thể tìm kiếm trên mạng để biết thêm về phần này. 
{{% /notice %}}

### Tạo cơ sở dữ liệu

- Trong giao diện **DynamoDB**, ta chọn **Create table** 
![ConnectPrivate](01AWSWorkShop/images/DynamoDB1.jpg)
- Trong giao diện **Create table**, ở phần **Table name** ta nhập tên bảng mong muốn, ở **Partition key** ta nhập tên key và chọn kiểu dữ liệu, **Sort key** có thể nhập hoặc không 
![ConnectPrivate](01AWSWorkShop/images/DynamoDB2.jpg)

- Còn lại ta để default hết rồi cuộn xuống chọn **Create table**
![ConnectPrivate](01AWSWorkShop/images/DynamoDB3.jpg)

- Đợi status lên **Active** sau đó ta chọn table vừa tạo, chọn **Action**, chọn **Explore items**
![ConnectPrivate](01AWSWorkShop/images/DynamoDB4.jpg)

- Trong giao diện **Explore items**, chọn **Create item**, **Partion key** chọn value tùy ý, các bạn chọn **Add new attribute** để thêm item, đặt tên tùy ý
![ConnectPrivate](01AWSWorkShop/images/DynamoDB5.jpg)
![ConnectPrivate](01AWSWorkShop/images/DynamoDB6.jpg)

Đến đây là ta đã tạo xong database để lưu số lượt xem rồi, mời các bạn sang bước tiếp theo.