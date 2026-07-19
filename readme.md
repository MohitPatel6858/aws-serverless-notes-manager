# 📒 AWS Serverless Notes Manager

<p align="center">

![AWS](https://img.shields.io/badge/AWS-Serverless-orange?logo=amazonaws)
![Amazon S3](https://img.shields.io/badge/Amazon-S3-569A31?logo=amazons3)
![AWS Lambda](https://img.shields.io/badge/AWS-Lambda-FF9900?logo=awslambda)
![API Gateway](https://img.shields.io/badge/API-Gateway-7B42BC)
![CloudWatch](https://img.shields.io/badge/Amazon-CloudWatch-FF9900)
![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![HTML5](https://img.shields.io/badge/HTML-5-E34F26?logo=html5)
![CSS3](https://img.shields.io/badge/CSS-3-1572B6?logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-success)

</p>

---

# 📌 Project Overview

AWS Serverless Notes Manager is a **Serverless Note Management Application** built using **Amazon API Gateway**, **AWS Lambda**, **Amazon S3**, and **Amazon CloudWatch**.

The application allows users to create and retrieve notes through a responsive web interface without managing any servers. Notes are securely stored as text files in Amazon S3 while AWS Lambda handles all backend operations. Amazon CloudWatch monitors requests and Lambda execution for debugging and performance tracking.

This project demonstrates how multiple AWS serverless services can be integrated to build a scalable, cost-effective, and fully serverless REST API application.

---

# 🚀 Live Demo

### 🌐 Website

**https://YOUR-S3-WEBSITE-LINK**

---

# 🏗️ AWS Architecture

<img src="https://github.com/user-attachments/assets/771a295c-c58e-43c0-8da1-579f580d66b5" width="100%">

---

# ✨ Features

- 📝 Create Notes
- 📖 Read Notes
- ☁️ Store Notes in Amazon S3
- ⚡ Serverless Backend using AWS Lambda
- 🌐 REST API with Amazon API Gateway
- 📊 CloudWatch Monitoring & Logging
- 📱 Responsive User Interface
- 🚀 Fast & Scalable Architecture

---

# 📸 Application Screenshots

## 🏠 Home Page

<img src="https://github.com/user-attachments/assets/5aa0c0f6-337a-465f-8f91-27572423de15">

---

## 📝 Note Saved Successfully

<img src="https://github.com/user-attachments/assets/86e9f0f6-5431-48ab-a938-33812f552e99">

---

## 📖 Read Note Successfully

<img src="https://github.com/user-attachments/assets/8c06d381-5600-4d54-ac07-f8d1e6abc863">

---

# ☁️ AWS Services Used

| Service | Purpose |
|---------|---------|
| Amazon S3 | Store Notes & Static Website Hosting |
| Amazon API Gateway | REST API Communication |
| AWS Lambda | Backend Business Logic |
| Amazon CloudWatch | Monitoring & Logging |
| AWS IAM | Permission Management |

---

# 🌐 Amazon S3

Amazon S3 is used for two purposes:

- Static Website Hosting
- Secure Storage of Notes as Text Files

<img src="https://github.com/user-attachments/assets/bb3493a8-687d-412b-ad3e-23fdf9c22868">

---

# 🚪 Amazon API Gateway

Amazon API Gateway exposes REST APIs for the frontend application and invokes AWS Lambda functions.

### REST APIs

- POST `/note`
- GET `/note`

---

# ⚡ AWS Lambda

The Lambda function performs all backend operations.

### Responsibilities

- Receive API Requests
- Validate Input
- Save Notes to Amazon S3
- Retrieve Notes from Amazon S3
- Return JSON Responses
- Handle Errors

<img src="https://github.com/user-attachments/assets/811f7ab4-4e85-4174-ac87-88e1988f3842">

---

# 📊 Amazon CloudWatch

Amazon CloudWatch captures Lambda execution logs, API requests, and application errors for monitoring and debugging.

<img src="https://github.com/user-attachments/assets/671c51be-8ab9-41b1-8096-c421adbfb5c6">

---

# 🔄 Project Workflow

```text
User

↓

Frontend (HTML, CSS, JavaScript)

↓

Amazon API Gateway

↓

AWS Lambda

├────────► Amazon S3
│
└────────► Amazon CloudWatch

↓

API Response

↓

Display Note to User
```

---

# 💻 Technology Stack

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- Python

### AWS Cloud

- Amazon API Gateway
- AWS Lambda
- Amazon S3
- Amazon CloudWatch
- AWS IAM

---

# 📂 Project Structure

```text
AWS-Serverless-Notes-Manager/

│── index.html
│── style.css
│── script.js
│── lambda_function.py
│── README.md
└── images/
```

---

# 📚 API Response

## Create Note

```json
{
  "message": "Note saved successfully."
}
```

## Read Note

```json
{
  "filename": "meeting.txt",
  "content": "Prepare AWS presentation."
}
```

---

# 📚 Learning Outcomes

This project helped me gain practical experience in:

- AWS Serverless Architecture
- Amazon API Gateway
- AWS Lambda
- Amazon S3 Object Storage
- Amazon CloudWatch Monitoring
- IAM Roles & Permissions
- REST API Development
- HTTP GET & POST Methods
- Static Website Hosting
- AWS Service Integration

---

# 🚀 Future Improvements

- ✏️ Edit Existing Notes
- 🗑️ Delete Notes
- 🔍 Search Notes by Filename
- 🔐 User Authentication using Amazon Cognito
- 🗃️ Store Metadata in Amazon DynamoDB
- 🌙 Dark Mode
- 📱 Enhanced Mobile Responsiveness

---

# 👨‍💻 Developer

## Mohit Patel

**B.Tech – Artificial Intelligence & Machine Learning**

AWS Cloud | Java

### Connect with Me

- GitHub: https://github.com/MohitPatel6858

---

# ⭐ Show Your Support

If you found this project useful or interesting, please consider giving this repository a ⭐ on GitHub.

Your support motivates me to build more AWS Cloud Projects.

---

## 📜 License

This project is developed for educational purposes and learning AWS Serverless technologies.
