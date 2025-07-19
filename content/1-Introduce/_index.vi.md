---
title : "Giới thiệu"
date: "2025-07-11"
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**CI/CD Pipeline Migration** là quá trình chuyển đổi hệ thống triển khai phần mềm từ mô hình cũ sang một pipeline hiện đại, hiệu quả hơn, đồng thời tích hợp nhiều công cụ để tự động hóa và tối ưu quy trình DevOps. Đề tài này sử dụng các dịch vụ của AWS như CodePipeline, CodeBuild, Elastic Beanstalk và CloudWatch nhằm xây dựng một quy trình triển khai tự động, linh hoạt và có khả năng giám sát chặt chẽ.
Việc tích hợp CI/CD vào quy trình phát triển giúp tăng tốc độ release, giảm thiểu lỗi khi triển khai và đảm bảo chất lượng phần mềm ổn định qua từng thay đổi trong mã nguồn. Đặc biệt, việc sử dụng các dịch vụ tích hợp sẵn của AWS giúp bạn dễ dàng mở rộng quy mô, cấu hình bảo mật và ghi log đầy đủ phục vụ việc giám sát và truy vết khi cần thiết.

Với việc thực hiện đề tài này, bạn sẽ đạt được những lợi ích sau:

- Tự động hóa toàn bộ quá trình build, test, và deploy khi có thay đổi trên GitHub.
- Không cần máy chủ trung gian (Bastion) để deploy thủ công.
- Tận dụng các dịch vụ serverless và managed của AWS giúp giảm chi phí vận hành.
- Giám sát và log chi tiết toàn bộ quá trình build/deploy bằng CloudWatch.
- Dễ dàng tích hợp thêm các công cụ kiểm thử hoặc phân tích mã nguồn như JUnit, SonarQube, v.v.
- Không cần SSH hoặc truy cập thủ công vào server, giúp đảm bảo an toàn bảo mật hệ thống.
- Quản lý và phân quyền triển khai theo IAM Role, đáp ứng các chính sách bảo mật nội bộ.
- Giao diện trực quan, dễ cấu hình, dễ mở rộng cho các nhóm phát triển lớn hoặc nhiều môi trường (dev/staging/production).

Với những ưu điểm trên, đề tài giúp thay thế các pipeline truyền thống, thủ công hoặc thiếu kiểm soát, bằng một giải pháp CI/CD hiện đại, tự động và đáng tin cậy trong môi trường AWS.


