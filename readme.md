# 📒 AWS Serverless Notes Manager

A **Serverless Notes Manager** built using **Amazon API Gateway, AWS Lambda, Amazon S3, and Amazon CloudWatch**. This project demonstrates how AWS serverless services work together to build a scalable and secure REST API for creating and retrieving notes without managing any servers.

---

## 🚀 Features

- 📝 Create notes using a **POST** REST API
- 📖 Read notes using a **GET** REST API
- ☁️ Store notes securely as text files in **Amazon S3**
- ⚡ Serverless backend powered by **AWS Lambda**
- 🌐 REST APIs exposed through **Amazon API Gateway**
- 📊 Monitor requests and errors using **Amazon CloudWatch**
- 💻 Responsive frontend built with **HTML, CSS & JavaScript**

---

## 🏗️ AWS Architecture

<img width="1536" height="1024" alt="AWS Architecture" src="https://github.com/user-attachments/assets/bc8e270d-8929-4e3d-bd25-c82efab999e9" />

---

## 🛠️ AWS Services Used

| Service | Purpose |
|---------|---------|
| Amazon API Gateway | Exposes REST API endpoints |
| AWS Lambda | Executes backend logic |
| Amazon S3 | Stores notes as text files |
| Amazon CloudWatch | Logs requests, responses, and errors |

---

## 💻 Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- Python

### AWS Services
- Amazon API Gateway
- AWS Lambda
- Amazon S3
- Amazon CloudWatch

### Tools
- Git
- GitHub

---

## 📡 API Endpoints

### 📝 Create Note

**POST** `/note`

#### Request Body

```json
{
  "filename": "meeting.txt",
  "content": "Prepare AWS presentation."
}
```

---

### 📖 Read Note

**GET**

```
/note?filename=meeting.txt
```

---

## 🔄 Project Workflow

```text
              User
                │
                ▼
     HTML / CSS / JavaScript
                │
                ▼
      Amazon API Gateway
                │
                ▼
         AWS Lambda (Python)
            │           │
            ▼           ▼
      Amazon S3    CloudWatch
```

---

# 📷 Project Screenshots

## 🏠 Home Page

<img width="1134" alt="Home Page" src="https://github.com/user-attachments/assets/cf37bea0-964b-40c5-83c5-86eeac39ecec" />

---

## 📝 Save Note Successfully

<img width="1112" alt="Save Note Successfully" src="https://github.com/user-attachments/assets/0063da9f-347f-4ad2-b21c-5c48810534e7" />

---

## 📖 Read Note Successfully

<img width="1434" alt="Read Note Successfully" src="https://github.com/user-attachments/assets/d85cc51c-aa5b-44ff-911c-bef6edf143bf" />

---

## ☁️ Amazon S3 Bucket

<img width="1544" alt="Amazon S3 Bucket" src="https://github.com/user-attachments/assets/be63c30a-b108-433e-a3c0-cc338be7a18f" />

---

## 📊 CloudWatch Logs

<img width="1622" alt="CloudWatch Logs" src="https://github.com/user-attachments/assets/4a6486d5-8c2b-43eb-b708-0c55317e84db" />

---

## ⚙️ AWS Lambda Function

<img width="706" alt="AWS Lambda Function" src="https://github.com/user-attachments/assets/ca009f1d-5a9b-433c-b9c7-71bdcaf9c537" />

---

## 🎯 Learning Outcomes

Through this project, I learned:

- Designing REST APIs with Amazon API Gateway
- Developing serverless applications using AWS Lambda
- Storing and retrieving files from Amazon S3
- Monitoring Lambda execution with Amazon CloudWatch
- Connecting a frontend application with AWS services
- Understanding and implementing Serverless Architecture
- Working with HTTP methods (GET and POST)
- Deploying and testing AWS-based applications

---

## 🚀 Future Improvements

- 🔐 User Authentication using Amazon Cognito
- ✏️ Edit existing notes
- 🗑️ Delete notes
- 🔍 Search notes by filename
- 🗃️ Amazon DynamoDB integration
- 📱 Improved mobile experience
- 🌙 Dark Mode

---

## 👨‍💻 Author

**Mohit Patel**

**B.Tech – Artificial Intelligence & Machine Learning (AIML)**

### Currently Learning

- ☁️ AWS Cloud
- ☕ Java
- 🌐 REST APIs
- 🛠️ Git & GitHub

### GitHub

**https://github.com/MohitPatel6858**

---

## ⭐ Support

If you found this project helpful or interesting, please consider giving it a **⭐ Star** on GitHub. Your support is appreciated!
