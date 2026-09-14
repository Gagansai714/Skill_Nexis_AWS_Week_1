# ☁️ AWS Cloud Computing Fundamentals & IAM/S3 Hands-On

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![IAM](https://img.shields.io/badge/AWS_IAM-DD344C?style=for-the-badge&logo=amazonaws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![Status](https://img.shields.io/badge/Submission-Completed-brightgreen?style=for-the-badge)

Welcome to the **Week 1 Assignment & Mini Project** repository for the Cloud Computing with AWS program. This project covers core cloud computing concepts, AWS account security configuration using IAM, key service architectures, and hosting static web assets via Amazon S3.

---

## 📌 Table of Contents
- [Assignment 1: Account Setup & Security](#-assignment-1-account-setup--security)
- [Assignment 2: Core AWS Services Report](#-assignment-2-core-aws-services-report)
- [Mini Project: IAM & S3 Hands-On](#-mini-project-iam--s3-hands-on)
- [Proof of Work & Screenshots](#-proof-of-work--screenshots)
- [Repository Structure](#-repository-structure)

---

## 🔐 Assignment 1: Account Setup & Security

1. **Free Tier Setup**: Created an AWS Free Tier account and secured root account credentials using Multi-Factor Authentication (MFA).
2. **IAM Configuration**: 
   * Avoided using the root account for daily operations.
   * Created a dedicated IAM User with tailored administrative access policies.
   * Configured user group policies and verified console login via custom IAM URL.

---

## 📋 Assignment 2: Core AWS Services Report

| Service | Category | Key Function & Primary Use Case |
| :--- | :--- | :--- |
| **Amazon EC2** | Compute | Scalable virtual servers in the cloud. Used for hosting applications, web servers, and backend compute workloads. |
| **Amazon S3** | Storage | Object storage built to store and retrieve any amount of data. Used for backup, static website hosting, and file storage. |
| **Amazon RDS** | Database | Managed relational database service (MySQL, PostgreSQL, etc.). Used for transactional application databases needing automated backups. |
| **AWS Lambda** | Serverless | Event-driven, serverless compute engine. Executes code in response to events without provisioning or managing servers. |

---

## 🛠️ Mini Project: IAM & S3 Hands-On

### 1. IAM User Provisioning
* Created a restricted IAM user `s3-admin-user` with `AmazonS3FullAccess` policy bindings.

### 2. S3 Bucket Deployment
* Provisioned an S3 Bucket with a globally unique name.
* Uploaded a static HTML asset (`index.html`) to the bucket root.

### 3. Public Access Policy Configuration
* Disabled the default **Block *all* public access** settings on the bucket.
* Applied the following JSON Bucket Policy to enable public `s3:GetObject` permissions:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::-/*"
    }
  ]
}
