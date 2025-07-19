---
title : "TẠO ELASTIC BEANSTALK"
date: "2025-07-11"
weight : 3 
chapter : false
pre : " <b> 3. </b> "
---


#### Tạo **ELASTIC BEANSTALK**
1. Truy cập **AWS Management Console** và mở dịch vụ **ELASTIC BEANSTALK**.

![VPC](/images/3.connect/001-BEAN.png)

2. Tại giao diện chính của **ELASTIC BEANSTALK** chọn **Create application**.

![VPC](/images/3.connect/002-BEAN.png)

3. Tại giao diện **Configure environment**.
  + Click **Web server environment**.
  + Đặt tên Application là ```nodejs-app```.
  + Đặt tên Environment là ```Nodejs-app-env```.
  + Trong **Platform** chọn Node.js.
  + Application code click **Sample application**.
  + Presets click **Single instance**
  + Click **Next**.

![VPC](/images/3.connect/003-BEAN.png)
![VPC](/images/3.connect/004-BEAN.png)

4. Tại giao diện **Configure service accesss**.
  + Tại **Service role** chọn role đã tạo **aws-elasticbeanstalk-service-role**.
  + Tại EC2 instance profile chon role đã tạo **aws-elasticbeanstalk-ec2-role**.
  + Click **Next**.

  ![VPC](/images/3.connect/005-BEAN.png)

5. Tại giao diện **Set up networking, database, and tags - optional**.
  + Kéo xuống chọn **Skip to review**.

  ![VPC](/images/3.connect/006-BEAN.png)
  ![VPC](/images/3.connect/007-BEAN.png)
6. Tại giao diện **Review**.
  + Click **Create**.

  ![VPC](/images/3.connect/008-BEAN.png)
  ![VPC](/images/3.connect/009-BEAN.png)

7. Sau khi tạo xong để xem trang thì chọn link dưới **Domain**.

  ![VPC](/images/3.connect/010-BEAN.png)
  ![VPC](/images/3.connect/011-BEAN.png)