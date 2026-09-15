# ☁️ AWS Cloud Computing Fundamentals & IAM/S3 Architecture

<div align="center">

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![IAM](https://img.shields.io/badge/AWS_IAM-DD344C?style=for-the-badge&logo=amazonaws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![Build Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

</div>

---

## 📌 Executive Summary
This repository contains the comprehensive submission for **Week 1: Introduction to Cloud Computing & AWS Basics**. It covers fundamental cloud computing models, account security configurations via **AWS IAM**, core service architectures, and a hands-on deployment of a static web application hosted on **Amazon S3** with custom bucket security policies.

---

## 🚀 Key Learning Outcomes & Technical Highlights
* **Cloud Architecture Foundations**: Evaluated IaaS, PaaS, SaaS, and deployment models.
* **Identity & Security (IAM)**: Implemented Least Privilege Principle by isolating root credentials and provisioning dedicated user groups.
* **Static Asset Hosting**: Configured public read permissions on Amazon S3 via JSON policies to host web assets.

---

## 📋 Assignment 1: Account & IAM Security Configuration

* **Root Account Hardening**: Configured AWS Free Tier account with Multi-Factor Authentication (MFA) enabled.
* **IAM User Provisioning**:
  * Created user `s3-admin-user` to handle daily infrastructure tasks.
  * Attached direct access policies (`AmazonS3FullAccess`) to manage object storage securely.
  * Verified isolation between root access and delegated IAM permissions.

---

## 🏛️ Assignment 2: Core AWS Services Architecture Report

| Service | Category | Core Functionality | Practical Use Case |
| :--- | :--- | :--- | :--- |
| **Amazon EC2** | Compute | Scalable virtual servers on demand | Hosting web servers, APIs, and scalable compute workloads. |
| **Amazon S3** | Storage | High-durability object storage | Storing assets, static site hosting, and backup/disaster recovery. |
| **Amazon RDS** | Database | Managed relational database engine | Handling transactional relational databases (MySQL, PostgreSQL). |
| **AWS Lambda** | Serverless | Event-driven compute execution | Running microservice functions without managing server infrastructure. |

---

## 🛠️ Mini-Project Implementation: IAM & S3 Deployment

### 1. Bucket Creation & Access Overrides
Created a General Purpose S3 bucket named `gagan-aws-demo-bucket` with public access restrictions removed to allow custom bucket policy assignment.

### 2. Live JSON Bucket Policy
Applied the following public read policy to grant `s3:GetObject` access across all objects:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::gagan-aws-demo-bucket/*"
    }
  ]
}
