---
title : "Tạo CodeBuild"
date: "2025-07-11"
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---


#### Tạo **CodeBuild**
1. Truy cập **AWS Management Console** và mở dịch vụ **CodeBuild**.
 
![VPC](/images/4.s3/001-CodeBuild.png)

2. Tại giao diện chính của **CodeBuild** chọn **Create project**.

![VPC](/images/4.s3/002-CodeBuild.png)

3. Tại giao diện **Create build project**.
  + Đặt tên project là ```*build-nodeappjs```.
  + Project type chon **Default project**.
  + Source chọn **Github**.

  ![VPC](/images/4.s3/003-CodeBuild.png)

  + Repository là link repository bạn đã tạo ở trên.
  + Chọn **Rebuild every time a code change is pushed to this repository**.
  + Ở Build type chọn **Single build**.

   ![VPC](/images/4.s3/004-CodeBuild.png)
  + Ở Environment chọn **On-demand** , **Managed image**, **EC2**, **Container** phần ở trong Environtment còn lại giữ nguyên.

  ![VPC](/images/4.s3/005-CodeBuild.png)

  + Chọn New **service role** và role name sẽ được tự động tạo.
  + Trong Buildspec chọn **Use a buildspec file**.

  ![VPC](/images/4.s3/006-CodeBuild.png)

  + Click **Create build project**.

  ![VPC](/images/4.s3/007-CodeBuild.png)
 



4. Dưới đây là giao diện sau khi tạo xong

![VPC](/images/4.s3/008-CodeBuild.png)