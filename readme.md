# 📒 AWS Serverless Notes Manager

A serverless web application built using **Amazon API Gateway**, **AWS Lambda**, **Amazon S3**, and **Amazon CloudWatch**. This project allows users to create and retrieve notes through REST APIs while demonstrating a complete serverless architecture on AWS.

---

## 🚀 Features

- 📝 Create notes using **POST /note**
- 📖 Read notes using **GET /note**
- ☁️ Store notes as text files in **Amazon S3**
- ⚡ Serverless backend using **AWS Lambda**
- 🌐 REST APIs with **Amazon API Gateway**
- 📊 Request and error logging with **CloudWatch**
- 💻 Responsive frontend using HTML, CSS & JavaScript

---

## 🏗️ Architecture

![AWS Architecture](images/architecture.png)

---

## 🛠️ AWS Services Used

| AWS Service | Purpose |
|-------------|---------|
| Amazon API Gateway | Handles REST API requests |
| AWS Lambda | Executes backend logic |
| Amazon S3 | Stores note files |
| Amazon CloudWatch | Logs API requests and errors |

---

## 💻 Technology Stack

- HTML5
- CSS3
- JavaScript
- Python
- AWS Lambda
- Amazon API Gateway
- Amazon S3
- Amazon CloudWatch
- Git
- GitHub

---

## 📂 Project Structure

```text
aws-serverless-notes-manager/
│
├── images/
│   ├── architecture.png
│   ├── home-page.png
│   ├── save-note-success.png
│   ├── read-note-success.png
│   ├── s3-bucket.png
│   ├── cloudwatch-logs.png
│   └── lambda-function.png
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## 📡 API Endpoints

### Create Note

**POST** `/note`

```json
{
  "filename": "meeting.txt",
  "content": "Prepare AWS presentation."
}
```

---

### Read Note

**GET** `/note?filename=meeting.txt`

---

## 🔄 Workflow

```
Frontend
      │
      ▼
Amazon API Gateway
      │
      ▼
 AWS Lambda
   │        │
   ▼        ▼
Amazon S3  CloudWatch
```

---

# 📷 Project Screenshots

## 🏠 Home Page

![Home Page](images/home-page.png)

---

## 📝 Save Note Successfully

![Save Note](images/save-note-success.png)

---

## 📖 Read Note Successfully

![Read Note](images/read-note-success.png)

---

## ☁️ Amazon S3 Bucket

![S3 Bucket](images/s3-bucket.png)

---

## 📊 CloudWatch Logs

![CloudWatch Logs](images/cloudwatch-logs.png)

---

## ⚙️ AWS Lambda Function

![Lambda Function](images/lambda-function.png)

---

## 🎯 Learning Outcomes

- Developed REST APIs using Amazon API Gateway
- Implemented backend logic with AWS Lambda
- Stored and retrieved files from Amazon S3
- Monitored application logs using CloudWatch
- Integrated a frontend with AWS serverless services
- Gained practical experience with Serverless Architecture

---

## 🚀 Future Enhancements

- User Authentication
- Edit & Delete Notes
- Search Notes
- DynamoDB Integration
- Dark Mode Support

---

## 👨‍💻 Author

**Mohit Patel**

B.Tech – Artificial Intelligence & Machine Learning (AIML)

🌐 GitHub: https://github.com/MohitPatel6858

---

⭐ **If you like this project, don't forget to Star the repository!**
