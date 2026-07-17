# 📒 AWS Serverless Notes Manager

A modern serverless web application built on **AWS** that allows users to create and retrieve notes using REST APIs. The application demonstrates how **Amazon API Gateway**, **AWS Lambda**, **Amazon S3**, and **Amazon CloudWatch** work together to build a scalable backend without managing servers.

---

## 📌 Project Overview

The application provides a simple web interface where users can:

- 📝 Create a note
- ☁️ Store the note as a `.txt` file in Amazon S3
- 📖 Retrieve any saved note
- 📊 Monitor API requests through CloudWatch Logs

This project demonstrates a real-world **Serverless Architecture** using AWS managed services.

---

# 🚀 Live Features

- ✅ Create Notes
- ✅ Read Notes
- ✅ Store notes in Amazon S3
- ✅ Retrieve notes from Amazon S3
- ✅ REST API using API Gateway
- ✅ AWS Lambda backend
- ✅ CloudWatch request logging
- ✅ Responsive Frontend
- ✅ Serverless Architecture

---

# 🏗️ System Architecture

```
                +----------------------+
                |      Frontend        |
                | HTML • CSS • JS      |
                +----------+-----------+
                           |
                           |
                    HTTP Request
                           |
                           ▼
                +----------------------+
                | Amazon API Gateway   |
                +----------+-----------+
                           |
                           ▼
                +----------------------+
                |     AWS Lambda       |
                |   Python Function    |
                +----------+-----------+
                           |
              +------------+------------+
              |                         |
              ▼                         ▼
     +----------------+        +--------------------+
     |   Amazon S3    |        | Amazon CloudWatch  |
     | Store Notes    |        | Logs & Monitoring  |
     +----------------+        +--------------------+
```

---

# 🛠️ AWS Services Used

| AWS Service | Purpose |
|-------------|---------|
| Amazon API Gateway | Exposes REST API endpoints |
| AWS Lambda | Executes backend logic |
| Amazon S3 | Stores notes as text files |
| Amazon CloudWatch | Logs API requests and errors |

---

# 💻 Technology Stack

- HTML5
- CSS3
- JavaScript (ES6)
- Python
- AWS Lambda
- Amazon API Gateway
- Amazon S3
- Amazon CloudWatch
- Git
- GitHub

---

# 📂 Project Structure

```
aws-serverless-notes-manager/
│
├── images/
│   ├── home-page.png
│   ├── save-note-success.png
│   ├── read-note-success.png
│   ├── s3-bucket.png
│   ├── cloudwatch-logs.png
│   └── architecture.png
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

# 📡 API Endpoints

## Create Note

**POST** `/note`

### Request

```json
{
    "filename": "meeting.txt",
    "content": "Prepare AWS presentation."
}
```

### Success Response

```json
{
    "message": "Note saved successfully."
}
```

---

## Read Note

**GET** `/note?filename=meeting.txt`

### Success Response

```json
{
    "filename": "meeting.txt",
    "content": "Prepare AWS presentation."
}
```

---

# 🔄 Application Workflow

### Step 1

The user enters a filename and note content from the web interface.

↓

### Step 2

The frontend sends an HTTP request to Amazon API Gateway.

↓

### Step 3

API Gateway invokes the AWS Lambda function.

↓

### Step 4

Lambda validates the request.

↓

### Step 5

The note is stored or retrieved from Amazon S3.

↓

### Step 6

CloudWatch automatically records every request and error.

↓

### Step 7

The response is displayed back to the user.

---

# 📷 Project Screenshots

## 🏠 Home Page

![Home Page](images/home-page.png)

---

## 📝 Create Note Successfully

![Create Note](images/save-note-success.png)

---

## 📖 Retrieve Note Successfully

![Read Note](images/read-note-success.png)

---

## ☁️ Amazon S3 Bucket

![Amazon S3](images/s3-bucket.png)

---

## 📊 CloudWatch Logs

![CloudWatch Logs](images/cloudwatch-logs.png)

---

## 🏗️ AWS Architecture

![Architecture](images/architecture.png)

---

# 🎯 Key Learning Outcomes

Through this project, I learned:

- Building REST APIs with Amazon API Gateway
- Writing backend logic using AWS Lambda
- Using Amazon S3 for object storage
- Monitoring applications with Amazon CloudWatch
- Integrating frontend with serverless backend
- Handling HTTP GET and POST requests
- Working with JSON data
- Building scalable serverless applications

---

# 📈 Future Enhancements

- User Authentication (Amazon Cognito)
- Update Existing Notes
- Delete Notes
- Search Notes
- DynamoDB Integration
- File Upload Support
- Responsive Dark Mode
- Note Categories
- User Dashboard

---

# ⚙️ Setup Instructions

### Clone Repository

```bash
git clone https://github.com/MohitPatel6858/aws-serverless-notes-manager.git
```

---

### Navigate into Project

```bash
cd aws-serverless-notes-manager
```

---

### Configure API Endpoint

Open `script.js`

Replace

```javascript
const API_BASE_URL = "YOUR_API_GATEWAY_URL";
```

with your deployed API Gateway endpoint.

---

### Run

Simply open

```
index.html
```

in your browser.

---

# 📚 Concepts Demonstrated

- Serverless Computing
- REST API
- Event-Driven Architecture
- Cloud Storage
- Object Storage
- Logging & Monitoring
- Frontend & Backend Integration
- AWS Cloud Services

---

# 👨‍💻 Author

**Mohit Patel**

B.Tech – Artificial Intelligence & Machine Learning (AIML)

### Currently Learning

- AWS Cloud
- Java
- Backend Development
- REST APIs
- Git & GitHub

**GitHub**

https://github.com/MohitPatel6858

---

# ⭐ Support

If you found this project helpful, please consider giving it a ⭐ on GitHub.

It motivates me to build more AWS and Cloud projects.
