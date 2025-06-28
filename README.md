# Data-Analyst-Knowladge-Ca  
# ☁️ AWS Learning Portfolio

This repository presents my practical case studies and findings from an AWS-focused course using the `Employee Exit Interviews.csv` dataset. Each module showcases specific AWS services through hands-on assignments. This prepared me not only to understand the concepts of AWS services but also to apply them in real-world scenarios while becoming more familiar with the AWS platform.

---

## 📝 Project Overview: HR Analytics with AWS

This project demonstrates how AWS cloud tools can be used to manage and analyze HR-related data, specifically focusing on employee exit interviews. By storing, processing, and securing the dataset on AWS, I explored practical implementations of infrastructure, automation, and access control.

### 🔍 Project Goals:
- Securely store and analyze HR data on the cloud.
- Automate tasks using serverless services.
- Estimate and optimize cost of cloud usage.
- Build a scalable, secure architecture for data analysis.

### 📦 Tools & Services Used:
- Amazon S3 (Data storage)
- AWS Athena (SQL querying)
- AWS Lambda (Automation)
- IAM (User access management)
- VPC (Private network)
- EC2 + EBS (Compute & storage)
- AWS Pricing Calculator (Cost estimation)

---

## 📚 Table of Contents

- [📦 Part 1: Core AWS Concepts](#-part-1-core-aws-concepts)
- [🔐 Part 2: AWS Services and Security](#-part-2-aws-services-and-security)

---

## 📦 Part 1: Core AWS Concepts

### 🧱 Module 1: AWS Deployment and Service Models

- ✅ **Case Study Result:**  
   ![Carlos A Portfolio-Module #1 drawio](https://github.com/user-attachments/assets/e7da3ee8-d15f-4f7c-aa31-d9c0d7925860)
  🖼️ *Screenshot Explanation:* This diagram shows the four main AWS deployment models (Public, Private, Hybrid, Community) and how each applies to different data needs. It also illustrates how SaaS, PaaS, and IaaS models interact with HR systems.

- 🧠 **Explanation:**  
  I explored AWS deployment models (Public, Private, Hybrid, Community) and service models (IaaS, PaaS, SaaS). For this HR dataset, a hybrid model is best, keeping sensitive data secure while leveraging cloud tools for analytics and scalability.

---

### 💸 Module 2: AWS Cost Analysis

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 2 drawio](https://github.com/user-attachments/assets/69f5c21c-1088-4647-baf9-4629df38ebe2)  
  🖼️ *Screenshot Explanation:* This screenshot shows the AWS Pricing Calculator setup, including S3 storage, Athena queries, and Lambda function usage. It highlights estimated monthly costs and usage details.

- 🧠 **Explanation:**  
  I used the AWS Pricing Calculator to estimate storage and querying costs. With Athena and S3, I saw how pricing is affected by data volume, DPU count, and query length. Using compressed data and serverless tools helped reduce costs.

---

### 🌍 Module 3: AWS Global Infrastructure

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 3 drawio](https://github.com/user-attachments/assets/e02927fc-5941-4d2e-98e9-a216ca36c35f)  
  🖼️ *Screenshot Explanation:* This image highlights the structure of AWS Regions, Availability Zones, and Edge Locations. It demonstrates how selecting Canada Central reduces latency for Canadian HR data.

- 🧠 **Explanation:**  
  I explored AWS’s global infrastructure and learned how to choose the optimal region for data hosting. For HR data in Canada, the Canada Central region provides low latency and ensures data residency compliance.

---

## 🔐 Part 2: AWS Services and Security

### 🔑 Module 4: AWS Identity and Access Management (IAM)

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 4 drawio](https://github.com/user-attachments/assets/5c474856-9b59-48c6-bb32-479196704ff8)  
  🖼️ *Screenshot Explanation:* This diagram shows the IAM configuration with Admin, Analyst, and Viewer roles, and their permission levels. It also includes example policy attachments for each role.

- 🧠 **Explanation:**  
  I created IAM users and policies that followed the principle of least privilege. For instance, an analyst user was granted read-only access to the S3 bucket storing the dataset, while an admin user had full access to AWS services. This exercise emphasized the importance of managing permissions to avoid data leaks or unauthorized access.

---

### 🌐 Module 5: AWS Virtual Private Cloud (VPC)

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 5 drawio](https://github.com/user-attachments/assets/0d3edf25-ab05-4402-99f7-275e8a9eb4b6)  
  🖼️ *Screenshot Explanation:* This VPC architecture diagram includes a public subnet (for access tools) and private subnets (for secure analytics), plus routing tables and a NAT Gateway to allow internet updates without exposing sensitive resources.

- 🧠 **Explanation:**  
  I set up a custom VPC with public and private subnets. The analysis tools accessing the `Employee Exit Interviews.csv` dataset were placed in private subnets, with NAT Gateway access to the internet for updates. This enhanced security while keeping the system scalable and reliable.

---

### ⚙️ Module 6: AWS Lambda

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 6 drawio](https://github.com/user-attachments/assets/9b37d0da-2634-4013-b992-ea7889264b0e)  
  🖼️ *Screenshot Explanation:* This diagram shows the event-driven architecture using Lambda. It triggers automatically when new files are uploaded to S3 and performs data preprocessing functions.

- 🧠 **Explanation:**  
  I built Lambda functions that trigger when new data is uploaded to S3. These functions clean and reformat the dataset automatically, showing how serverless automation saves time and reduces infrastructure complexity.

---

### 💾 Module 7: AWS Elastic Block Store (EBS)

- ✅ **Case Study Result:**  
  ![Carlos A Portfolio-Module 7 drawio](https://github.com/user-attachments/assets/cc863776-f5e5-4060-9505-560633af0607)  
  🖼️ *Screenshot Explanation:* This screenshot shows the EBS volume attached to an EC2 instance running data analysis tasks. It includes info about volume type, size, and snapshot configuration.

- 🧠 **Explanation:**  
  I provisioned EBS volumes for EC2-based data processing. This helped simulate running larger workloads on AWS. I tested volume types (gp3 vs io1) and took snapshots to secure and manage persistent storage.

---

