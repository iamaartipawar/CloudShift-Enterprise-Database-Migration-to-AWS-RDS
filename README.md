# **🛢️ CloudShift: Enterprise Database Migration to AWS RDS**
- Database Transformation Journey: From Self-Managed Infrastructure to Amazon RDS

## **📖 About The Project**

Modern cloud applications require scalable and managed database solutions. This project demonstrates migrating a self-managed MariaDB database running on an EC2 instance to Amazon RDS while preserving database structure and records.

The project simulates a real-world migration scenario where traditional infrastructure is transformed into managed cloud infrastructure.

## **🏗️ Architecture Diagram**

<p align="center">
  <img src="images/Architec.png" width="700">
</p>

---

## **⚙️ Tech Stack**

- AWS EC2
- Amazon RDS
- MariaDB
- Linux
- SQL
- AWS Security Groups

## **⚡ Project Workflow**
### **🔹Step 1 : Traditional Database Setup**

✔ Launched EC2 instance named Traditional DB

✔ Installed and configured MariaDB

✔ Created local database environment

✔ Configure the Security group

<p align="center">
  <img src="images/1.png" width="700">
</p>

---

<p align="center">
  <img src="images/2.png" width="700">
</p>

---

<p align="center">
  <img src="images/25.png" width="700">
</p>

---

<p align="center">
  <img src="images/3.png" width="700">
</p>

---

<p align="center">
  <img src="images/4.png" width="700">
</p>

---

<p align="center">
  <img src="images/5.png" width="700">
</p>

---

<p align="center">
  <img src="images/6.png" width="700">
</p>

---

<p align="center">
  <img src="images/7.png" width="700">
</p>

---

<p align="center">
  <img src="images/8.png" width="700">
</p>

---

<p align="center">
  <img src="images/9.png" width="700">
</p>

---


### **🔹 Step 2 : Amazon RDS Deployment**

✔ Created MariaDB RDS 

✔ Configured database access

✔ Extract data from db

- mysqldump -u root -p insta > insta_bkp.sql

✔ Migrate from EC2 to RDS
- <endpoint> insta < insta_bkp.sql

✔ Configured security groups

<p align="center">
  <img src="images/10.png" width="700">
</p>

---

<p align="center">
  <img src="images/11.png" width="700">
</p>

---

<p align="center">
  <img src="images/12.png" width="700">
</p>

---

<p align="center">
  <img src="images/13.png" width="700">
</p>

---

<p align="center">
  <img src="images/14.png" width="700">
</p>

---

<p align="center">
  <img src="images/24.png" width="700">
</p>

---

<p align="center">
  <img src="images/15.png" width="700">
</p>

---

<p align="center">
  <img src="images/16.png" width="700">
</p>

---

<p align="center">
  <img src="images/17.png" width="700">
</p>

---

<p align="center">
  <img src="images/18.png" width="700">
</p>

---

<p align="center">
  <img src="images/19.png" width="700">
</p>

---

<p align="center">
  <img src="images/20.png" width="700">
</p>

---

<p align="center">
  <img src="images/21.png" width="700">
</p>

---

<p align="center">
  <img src="images/22.png" width="700">
</p>

---

<p align="center">
  <img src="images/23.png" width="700">
</p>

---
### **🔹 Step 3 : Create Read Replica**
- Select the Primary RDS instance.
- Create a Read Replica.
- Wait until replication status becomes Available.
- Verify replicated data by connecting to the replica.

<p align="center">
  <img src="images/26.png" width="700">
</p>

<p align="center">
  <img src="images/27.png" width="700">
</p>

<p align="center">
  <img src="images/28.png" width="700">
</p>

<p align="center">
  <img src="images/29.png" width="700">
</p>

<p align="center">
  <img src="images/30.png" width="700">
</p>


## **🚀 Migration Achievements**

✔ Successfully migrated database workloads from traditional infrastructure to Amazon RDS

✔ Maintained database structure and records during migration

✔ Established secure connectivity between EC2 and Amazon RDS

✔ Demonstrated real-world database modernization using AWS services

## **🎯 Project Outcome**

- Successfully migrated the database from EC2 to Amazon RDS.
- Configured secure communication between EC2 and RDS.
- Successfully created an Amazon RDS Read Replica.
- Verified automatic data replication.
- Improved database read performance and scalability using Read Replica.

## **🚀 Future Enhancements**
- Enable Multi-AZ deployment
- Configure automated backups
- Implement CloudWatch monitoring
- Automate deployment using Terraform
- Integrate CI/CD pipeline
- Enable RDS Performance Insights
