# 📒 AWS Serverless Notes Manager

A **Serverless Notes Manager** built using **Amazon API Gateway, AWS Lambda, Amazon S3, and Amazon CloudWatch**. This project demonstrates how AWS serverless services work together to build a scalable REST API for creating and retrieving notes without managing any servers.

---

## 🚀 Features

- 📝 Create notes using **POST API**
- 📖 Read notes using **GET API**
- ☁️ Store notes as text files in **Amazon S3**
- ⚡ Serverless backend using **AWS Lambda**
- 🌐 REST APIs with **Amazon API Gateway**
- 📊 Monitor API requests using **Amazon CloudWatch**
- 💻 Responsive frontend built with **HTML, CSS & JavaScript**

---

## 🏗️ AWS Architecture


<img width="1536" height="1024" alt="architecture" src="https://github.com/user-attachments/assets/bc8e270d-8929-4e3d-bd25-c82efab999e9" />

---

## 🛠️ AWS Services Used

| Service | Purpose |
|---------|---------|
| Amazon API Gateway | Exposes REST API endpoints |
| AWS Lambda | Executes backend logic |
| Amazon S3 | Stores notes as text files |
| Amazon CloudWatch | Logs requests and errors |

---

## 💻 Tech Stack

- HTML5
- CSS3
- JavaScript
- Python
- Amazon API Gateway
- AWS Lambda
- Amazon S3
- Amazon CloudWatch
- Git
- GitHub

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

### Read Note

**GET** `/note?filename=meeting.txt`

---

## 🔄 Project Workflow

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

<img width="1134" alt="Home Page" src="https://github.com/user-attachments/assets/cf37bea0-964b-40c5-83c5-86eeac39ecec" />

---

## 📝 Save Note Successfully

<img width="1112" alt="Save Note" src="https://github.com/user-attachments/assets/0063da9f-347f-4ad2-b21c-5c48810534e7" />

---

## ☁️ Amazon S3 Bucket

<img width="1544" alt="Amazon S3 Bucket" src="https://github.com/user-attachments/assets/be63c30a-b108-433e-a3c0-cc338be7a18f" />

---

## 📊 CloudWatch Logs

<img width="1622" alt="CloudWatch Logs" src="https://github.com/user-attachments/assets/4a6486d5-8c2b-43eb-b708-0c55317e84db" />

---

## ⚙️ AWS Lambda Function

<img width="706" alt="Lambda Function" src="https://github.com/user-attachments/assets/ca009f1d-5a9b-433c-b9c7-71bdcaf9c537" />

---

## 🎯 Learning Outcomes

Through this project, I learned:

- Building REST APIs using Amazon API Gateway
- Developing serverless applications with AWS Lambda
- Storing and retrieving files from Amazon S3
- Monitoring applications using Amazon CloudWatch
- Integrating frontend applications with AWS services
- Understanding Serverless Architecture

---

## 🚀 Future Improvements

- User Authentication
- Edit & Delete Notes
- Search Functionality
- Amazon DynamoDB Integration
- Dark Mode Support

---

## 👨‍💻 Author

**Mohit Patel**

**B.Tech – Artificial Intelligence & Machine Learning (AIML)**

Currently Learning:
- AWS Cloud
- Java
- REST APIs
- Git & GitHub

GitHub: **https://github.com/MohitPatel6858**

---

⭐ **If you found this project useful, please consider giving it a Star!**
