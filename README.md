# ☁️ AWS Cloud Computing Fundamentals & IAM/S3 Architecture

> **BeeSkilled – Cloud Computing with AWS | Week 1 Assignment**
> 🚀 Foundations of Cloud Computing, IAM Security Configurations, and Static Asset Hosting via Amazon S3.

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![IAM](https://img.shields.io/badge/AWS_IAM-DD344C?style=for-the-badge&logo=amazonaws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Documentation](https://img.shields.io/badge/Documentation-Markdown-informational?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📌 Project Overview

This repository contains the comprehensive submission for **Week 1: Introduction to Cloud Computing & AWS Basics**. It demonstrates core cloud computing models, security governance using **AWS IAM**, key architectural services, and a practical deployment of a static web application hosted on **Amazon S3** utilizing custom bucket security policies.

Instead of basic file storage, this project follows cloud security best practices by isolating root privileges, configuring dedicated IAM user roles, and applying granular JSON access control policies to host public assets securely.

---

## 📚 Table of Contents

* 📌 Project Overview
* 🎯 Project Objectives
* 📌 Project Status
* ✨ Key Features
* 🛠️ Technologies & Tools
* 📂 Repository Structure
* 🔐 Assignment 1: Account & IAM Setup
* 🏛️ Assignment 2: Core AWS Services Report
* 🛠️ Mini-Project: IAM & S3 Deployment
* 🖼️ Proof of Work & Screenshots
* 📊 Repository Information
* 💡 Skills Demonstrated
* 🎓 Learning Outcomes
* 👨‍💻 Author
* 🙏 Acknowledgement
* ⭐ Support

---

## 📌 Project Status

✅ AWS Free Tier Account Provisioned

✅ IAM User & Access Roles Configured

✅ Core AWS Services Analysis Completed

✅ S3 General Purpose Bucket Deployed

✅ Public JSON Bucket Policy Applied

✅ Static File Hosted & Verified via S3 URL

✅ Documentation & Screenshots Completed

---

## 🎯 Project Objectives

* Master fundamental cloud models (IaaS, PaaS, SaaS) and deployment structures.
* Secure AWS cloud environments using Identity and Access Management (IAM).
* Analyze primary AWS compute, storage, database, and serverless services.
* Provision and configure Amazon S3 buckets for static web asset distribution.
* Write and apply custom JSON bucket policies for public `s3:GetObject` actions.
* Build professional project documentation for cloud infrastructure deployment.

---

## ✨ Key Features

* 🔐 **IAM Security Governance**: Configured dedicated IAM user with specific policy attachments.
* 🌐 **Static Web Hosting**: Deployed web assets directly to Amazon S3.
* 📜 **JSON Policy Control**: Configured custom resource access policies for S3 bucket objects.
* 📑 **Structured Documentation**: Clean markdown organization featuring full deployment proofs.

---

## 🛠️ Technologies & Tools

| Tool / Service | Category | Purpose |
| :--- | :--- | :--- |
| **AWS Console** | Cloud Platform | Central management interface for AWS resources |
| **AWS IAM** | Security & Identity | Access management, user roles, and security policies |
| **Amazon S3** | Cloud Storage | Object storage and static web file hosting |
| **HTML5** | Web Development | Static web interface source asset |
| **JSON** | Configuration | S3 bucket access policy definition |
| **Git & GitHub** | Version Control | Source code management and submission hosting |

---

## 📂 Repository Structure

```text
aws-cloud-computing-week1/
├── index.html            # Static HTML file deployed to Amazon S3
├── bucket-policy.json    # Public JSON Bucket Policy applied to gagan-aws-demo-bucket
├── README.md             # Detailed assignment report and proof of work
└── screenshots/          # Console verification images
    ├── iam-user-setup.png
    ├── s3-bucket-objects.png
    ├── s3-bucket-policy.png
    └── live-s3-website.png
