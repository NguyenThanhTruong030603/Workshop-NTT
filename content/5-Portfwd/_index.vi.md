---
title : "Tạo CodePipeline"
date: "2025-07-11"
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

#### Tạo **CodePipeline**
1. Truy cập **AWS Management Console** và mở dịch vụ **CodePipeline**.
  

![VPC](/images/5.fwd/001-CodePipeline.png)

2. Tại giao diện chính của **CodePipeline** chọn **Create pipeline**.
  
  ![VPC](/images/5.fwd/002-CodePipeline.png)



3. Tại giao diện **Choose creation option**.
  + Click **Build custom pipeline**.
  + Click **Next**.

  ![VPC](/images/5.fwd/003-CodePipeline.png)


4. Tại giao diện **Choose pipeline settings**.
  + Đặt tên pipeline là ```pipeline-nodejsapp```.
  + **Execution mode** chọn **Queued**.
  + Service role chọn **New service role**.
  + Click **Next**.

  ![VPC](/images/5.fwd/004-CodePipeline.png)

5. Tại giao diện **Add source stage**.
  + Tại source provider chọn **Github (via Github App)**.
  + Sau đó kết nối với Github của bạn.
  + Repositoy name điền tên repository bạn đã tạo.
  + Chọn branch lưu code của bạn.
  + Click **Next**.

  ![VPC](/images/5.fwd/005-CodePipeline.png)
  ![VPC](/images/5.fwd/006-CodePipeline.png)

6. Tại giao diện **Add Build stage**.
  + Chọn **Other build providers**.
  + Chọn **AWS CodeBuild**.
  + Chọn CodeBuild đã tạo khi nãy.
  + Build type chọn **Single build**
  + Click **Next**.

  ![VPC](/images/5.fwd/007-CodePipeline.png)
  ![VPC](/images/5.fwd/008-CodePipeline.png)

7. Tại giao diện **Add test stage**.
  + Click **Next**.

  ![VPC](/images/5.fwd/009-CodePipeline.png)

8. Tại giao diện **Add deploy stage**.
  + Chọn **AWS Elastic Beanstalk**.
  + Chọn Application name đã tạo ở **Elastic Beanstalk**.
  + Chọn Environment name đã tạo ở **Elastic Beanstalk**.
  + Click **Next**.

  ![VPC](/images/5.fwd/010-CodePipeline.png)

9. Tại Review kéo xuống chọn **Create pipeline**.

![VPC](/images/5.fwd/011-CodePipeline.png)
![VPC](/images/5.fwd/012-CodePipeline.png)

10. Dưới đây là giao diện tạo thành công.

  ![VPC](/images/5.fwd/013-CodePipeline.png)
11. Vào lại link Domain ở **Elastic Beanstalk** để xem trang đã deploy lên
    ![VPC](/images/5.fwd/014-CodePipeline.png)

Lưu ý: Nếu tạo thất bại thì hãy vào IAM chọn role và tìm role pipeline đang chạy hiện tại sau đó thêm role **AdministratorAccess-AWSElasticBeanstalk** rồi chọn Release change để chạy lại.

![VPC](/images/5.fwd/015-CodePipeline.png)
![VPC](/images/5.fwd/016-CodePipeline.png)
![VPC](/images/5.fwd/017-CodePipeline.png)
![VPC](/images/5.fwd/018-CodePipeline.png)
![VPC](/images/5.fwd/019-CodePipeline.png)