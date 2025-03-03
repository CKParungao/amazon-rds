# ☁️ Get Started: Setting Up a Relational Database in Amazon RDS ☁️

Project Overview

Image

**Disclaimer:** This activity is based on Sanjeev Thiyagarajan's [tutorial](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421).

## 📋 Requirements
1. **Browser** (Google Chrome, Microsoft Edge, Opera GX, etc.)
2. **AWS Account**
3. **pgAdmin 4**

## 🎯 Objectives
1. **Create an RDS Instance** and configure security for access.
2. **Define database schemas and tables.**
3. **Launch an EC2 Instance** for hosting the app.
4. **Connect the app to RDS** using the connection string.

## ✒️ Part 1: Create an RDS Instance and configure security for access.
1. Log in to your AWS Console.
2. Navigate to `RDS` then click the `Create database` button.
3. Select `Standard create` for the database creation method.
4. Click `PostgreSQL` for the engine type and retain the default engine version.
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

16. 


## ✒️ Part 2: Define database schemas and tables.


## ✒️ Part 3: Launch an EC2 Instance for hosting the app.


## ✒️ Part 4: Connect the app to RDS using the connection string.


## 📚 Authors
### Activity and Code Materials
- Sanjeev Thiyagarajan ([KodeKloud](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421))
### Learning Material
- Crystal Katherine Parungao ([CKParungao](https://github.com/CKParungao))
