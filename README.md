# Data-Analyst-Knowladge-Ca
# AWS Learning Portfolio

This repository presents my practical case studies and findings from an AWS-focused course using the `Employee Exit Interviews.csv` dataset. Each module showcases specific AWS services through hands-on assignments. This prepared me not only to understand the concepts of AWS services but to learn how to put them into practice and get familiar with the AWS platform. Next, I will be including insights and explanations of each of the steps I went through.

---

## 📦 Part 1: Core AWS Concepts

### Module 1: AWS Deployment and Service Models
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module #1 drawio](https://github.com/user-attachments/assets/ea177658-05ca-4c07-8fe3-bb22aca75034)

- 🧠 **Explanation:**  
  In this module, I explored different AWS deployment models (Public, Private, Hybrid, and Community) and service models (IaaS, PaaS, SaaS). By analyzing the Employee Exit Interviews dataset, I evaluated which deployment model would best suit a data analysis platform for HR analytics. A hybrid cloud model would allow sensitive employee data to be handled securely while leveraging public cloud scalability for storage and processing.

---

### Module 2: AWS Cost Analysis
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 2 drawio](https://github.com/user-attachments/assets/69f5c21c-1088-4647-baf9-4629df38ebe2)

- 🧠 **Explanation:**  
  I used the AWS Pricing Calculator to estimate the cost of storing and analyzing the dataset using services like S3, Athena, and Lambda. I found that using serverless services and querying compressed data in S3 using Athena helped minimize costs. I also learned how DPU (Data Processing Units) and query duration directly impact costs.

---

### Module 3: AWS Global Infrastructure
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 3 drawio](https://github.com/user-attachments/assets/e02927fc-5941-4d2e-98e9-a216ca36c35f)

- 🧠 **Explanation:**  
  In this section, I evaluated the distribution of AWS regions and availability zones. I learned that choosing the right region close to data sources (e.g., US West or Canada Central for this dataset) helps reduce latency and ensures compliance. I also understood how edge locations can improve delivery speed for any dashboards or insights shared with stakeholders.

---

## 🔐 Part 2: AWS Services and Security

### Module 4: AWS Identity and Access Management (IAM)
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 4 drawio](https://github.com/user-attachments/assets/5c474856-9b59-48c6-bb32-479196704ff8)

- 🧠 **Explanation:**  
  I created IAM users and policies that followed the principle of least privilege. For instance, an analyst user was granted read-only access to the S3 bucket storing the dataset, while an admin user had full access to AWS services. This exercise emphasized the importance of managing permissions to avoid data leaks or unauthorized access.

---

### Module 5: AWS Virtual Private Cloud (VPC)
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 5 drawio](https://github.com/user-attachments/assets/0d3edf25-ab05-4402-99f7-275e8a9eb4b6)

- 🧠 **Explanation:**  
  I set up a custom VPC with public and private subnets. The analysis tools accessing the `Employee Exit Interviews.csv` dataset were placed in private subnets, with NAT Gateway access to the internet for updates. This enhanced security while keeping the system scalable and reliable.

---

### Module 6: AWS Lambda
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 6 drawio](https://github.com/user-attachments/assets/9b37d0da-2634-4013-b992-ea7889264b0e)

- 🧠 **Explanation:**  
  I used AWS Lambda to automate data processing tasks on the exit interview data. For example, Lambda functions were triggered upon file upload to S3 to clean the data and standardize formats. This showed the power of event-driven, serverless computing for lightweight, repeated tasks without provisioning servers.

---

### Module 7: AWS Elastic Block Store (EBS)
- ✅ **Case Study Result:** ![Carlos A Portfolio-Module 7 drawio](https://github.com/user-attachments/assets/cc863776-f5e5-4060-9505-560633af0607)

- 🧠 **Explanation:**  
  This module involved provisioning EBS volumes and attaching them to EC2 instances for data processing tasks. I simulated analyzing larger chunks of the dataset on EC2 with persistent EBS storage. I learned about volume types (gp3 vs io1), snapshots, and optimizing storage performance vs. cost.

---



