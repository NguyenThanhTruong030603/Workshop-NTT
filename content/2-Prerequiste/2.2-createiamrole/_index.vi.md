---
title : "Tạo IAM Role"
date: "2025-07-11"
weight : 2 
chapter : false
pre : " <b> 2.2 </b> "
---

### Tạo IAM Role

Trong bước này chúng ta sẽ tiến hành tạo IAM Role.

1. Truy cập vào [giao diện quản trị dịch vụ IAM](https://console.aws.amazon.com/iamv2/)
2. Ở thanh điều hướng bên trái, click  **Roles**.  

![role](/images/2.prerequisite/001-IAMROLE.png)

3. Click **Create role**.  

![role1](/images/2.prerequisite/002-IAMROLE.png)

4. Click **AWS service** và click **Elastic Beanstalk** ở Use case. 
  + Click **Elastic Beanstalk - Compute**.
  + Click **Next**.  

![role1](/images/2.prerequisite/003-IAMROLE.png)

5. Trong **Add permissions**.
  + Kiểm tra phải có các policy: **AWSElasticBeanstalkMulticontainerDocker**, **AWSElasticBeanstalkWebTier**, **AWSElasticBeanstalkWorkerTier**.
  + Click **Next.**

![createpolicy](/images/2.prerequisite/004-IAMROLE.png)

6. Đặt role name là ```aws-elasticbeanstalk-ec2-role```, sau đó chọn **Create role**.
  + Click **Create Role**.

 ![createpolicy](/images/2.prerequisite/005-IAMROLE.png)
  ![createpolicy](/images/2.prerequisite/006-IAMROLE.png)
7. Tiếp tục ở **role** tạo tiếp 1 role mới.  
  + Click **Create Role**.

 ![role1](/images/2.prerequisite/002-IAMROLE.png)

8. Click **AWS service** và click **Elastic Beanstalk** ở Use case. 
  + Click **Elastic Beanstalk - Environtment**.
  + Click **Next**. 

  ![createpolicy](/images/2.prerequisite/007-IAMROLE.png)

9. Trong **Add permissions**.
  + Kiểm tra phải có các policy: **AWSElasticBeanstalkEnhancedHealth**, **AWSElasticBeanstalkManagedUpdatesCustomerRolePolicy**.
  + Click **Next.**

  ![namerole](/images/2.prerequisite/008-IAMROLE.png)

10. Đặt role name là ```aws-elasticbeanstalk-service-role```, sau đó chọn **Create role**.

![namerole](/images/2.prerequisite/009-IAMROLE.png)
![namerole](/images/2.prerequisite/010-IAMROLE.png)


