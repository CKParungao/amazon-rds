![image](https://github.com/user-attachments/assets/52044f0d-5c94-4e89-8b9d-09b487b9bd7f)# ☁️ Get Started: Setting Up a Relational Database in Amazon RDS ☁️

Project Overview

Image

**Disclaimer:** This activity is based on Sanjeev Thiyagarajan's [tutorial](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421).

## 📋 Requirements
1. **Browser** (Google Chrome, Microsoft Edge, Opera GX, etc.)
2. **AWS Account**
3. **pgAdmin 4**

## 🎯 Objectives
1. **Create an RDS Instance** and configure security for access.
2. **Connect the App to RDS** using the connection string.

## ✒️ Part 1: Create an RDS Instance and configure security for access.
1. Log in to your AWS Console.
2. Navigate to `RDS` then click the `Create database` button.
3. Select `Standard create` for the database creation method.
4. Click `PostgreSQL` for the engine type and retain the default engine version.

![image](https://github.com/user-attachments/assets/d559c966-bdd4-4dc3-8e6f-575956a28b85)

5. Choose `Free tier` for the template.
6. Automatically, the deployment option should be for a `Single-AZ DB instance deployment (1 instance)` only.
7. Type `my-first-db` for the DB instance identifier.
8. The master username should be `postgres` as the default. Meanwhile, provide the master password `masterpw`.
9. The DB instance class `db.t4g.micro` should be left in default.
10. In Storage, use the minimum `20` GiB for the allocated storage. Expand `Additional storage configuration` and then tick the checkbox of `Enable storage autoscaling`.

![image](https://github.com/user-attachments/assets/57ec6db5-a30e-4887-807d-6fcd72facf22)

11. Move onto the Connectivity section and set the Public access to `Yes`.

![image](https://github.com/user-attachments/assets/cd3ce6aa-62ee-4cbb-b564-3c012419d5a4)

12. In the VPC security group (firewall), choose `Create new` and type `my-db-sg` in the New VPC security group name.
13. Finally, click `Create database`.
14. Once the Status of the database turns to Available, click on `my-first-db`.

![image](https://github.com/user-attachments/assets/4ef215c5-6f49-496a-9404-a9a382f8201a)

15. Copy the `Endpoint`.

![image](https://github.com/user-attachments/assets/c2ae0f0d-4507-48ff-acae-9c6f3585814c)

16. Provide the sample connection details in the JS file `index.js`.

![image](https://github.com/user-attachments/assets/1f3bd768-6e56-4b12-90da-92932fd13f07)

## ✒️ Part 2: Connect the App to RDS using the connection string.

17. Launch the pgAdmin application in your desktop.
18. On the left tab, right-click on `Servers` and select `Register`->`Server`.
19. Type `aws-rds` for the server name.
20. On the Connection tab, paste the copied endpoint from RDS instance.

![image](https://github.com/user-attachments/assets/d37f6d74-20e4-453c-9eb1-6fe4b04f163f)

21. Type in `masterpw` for the Password then click the `Save` button.
22. Expand `aws-rds`. Right-click on `Databases` then select `Create`->`Database`
23. Use `myapp` as the Database name then click the `Save` button.
24. 

## 📚 Authors
### Activity and Code Materials
- Sanjeev Thiyagarajan ([KodeKloud](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421))
### Learning Material
- Crystal Katherine Parungao ([CKParungao](https://github.com/CKParungao))
