---
title : "DNS VỚI ROUTE53"
date :  "`r Sys.Date()`" 
weight : 4 
chapter : false
pre : " <b> 2.4. </b> "
---

{{% notice warning %}}
Chi phí để hoàn thiện bước này sẽ vào khoảng 3 dollar, các bạn có thể bỏ qua phần này và đi đến phần tiếp sau.
{{% /notice %}}

Sau khi hoàn thành phần trước chúng ta coi như là đã dựng thành công website sơ yếu lý lịch của bản thân, nhưng chúng ta bắt buộc phải dùng domain mặc định của **ClouFront**, nói chung khá là xấu, phức tạp và không theo ý của chúng ta. Để có thể sở hữu riêng một DNS theo ý bản thân, ở phần này mình sẽ hướng dẫn các bạn sử dụng dịch vụ **Route53**.
{{% notice note %}}
Các bạn có thể sử dụng DNS của các nhà cung cấp khác ngoài **AWS** cũng được, nhưng phải chuyển đổi một số thứ, các bạn có thể tìm kiếm trên mạng về vấn đề này. 
{{% /notice %}}


### Giới thiệu

 DNS – Domain Name System là một hệ thống quản lý các tên miền và ánh xạ chúng thành địa chỉ IP của máy chủ, cho phép các ứng dụng truy cập vào các dịch vụ trên internet bằng tên miền thay vì sử dụng địa chỉ IP.
 
 AWS Route 53 là một dịch vụ quản lý tên miền và DNS (Domain Name System) được cung cấp bởi Amazon Web Services (AWS). DNS AWS Route 53 cho phép bạn đăng ký và quản lý tên miền, tạo và cấu hình các bản ghi DNS, và điều hướng các yêu cầu từ tên miền đến các nguồn tài nguyên khác nhau trên AWS và bên ngoài. Điều này bao gồm điều hướng yêu cầu đến máy chủ web, máy chủ email, CDN và các tài nguyên khác.

 Route 53 cung cấp một loạt tính năng như đám mây DNS, chống chịu tải, đám mây phân phối nội dung, bảo mật và theo dõi tình trạng tài nguyên. Nó cũng tích hợp tốt với các dịch vụ khác của AWS, cho phép bạn tự động cập nhật bản ghi DNS khi tạo hoặc xoá các nguồn tài nguyên trên AWS.

**Các bước thực hiện**
1. [Mua Domain Name](2.4.1-BuyDNS/)

2. [Trỏ domain name tới CloudFront](2.4.2-DNSCloudFront/)

