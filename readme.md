<img width="1536" height="1024" alt="aws-serverless-notes-manager architecture" src="https://github.com/user-attachments/assets/771a295c-c58e-43c0-8da1-579f580d66b5" /># 📒 AWS Serverless Notes Manager

A **Serverless Notes Manager** built using **AWS Lambda**, **Amazon API Gateway**, **Amazon S3**, and **Amazon CloudWatch**. This project demonstrates how AWS serverless services work together to build a scalable REST API that allows users to create and retrieve notes without managing any servers.

---

## 🚀 Features

- 📝 Create notes using **POST** API
- 📖 Retrieve notes using **GET** API
- ☁️ Store notes securely in **Amazon S3**
- ⚡ Serverless backend powered by **AWS Lambda**
- 🌐 REST API using **Amazon API Gateway**
- 📊 Monitor API requests and execution logs using **Amazon CloudWatch**
- 🎨 Responsive and modern frontend
- 🚀 Fast, scalable, and fully serverless architecture

---

## 🛠️ Tech Stack

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

---

# 🏗️ Project Architecture

<img width="1536" alt="AWS Serverless Notes Manager Architecture" src="https://github.com/user-attachments/assets/771a295c-c58e-43c0-8da1-579f580d66b5" />

---

# 📂 Project Structure

```text
AWS-Serverless-Notes-Manager/
│
├── index.html
├── style.css
├── script.js
├── lambda_function.py
├── README.md
└── images/
```

---

# 📷 Project Screenshots

## 🏠 Home Page

<img width="1020" alt="Home Page" src="https://github.com/user-attachments/assets/5aa0c0f6-337a-465f-8f91-27572423de15" />

---

## 📝 Note Saved Successfully

<img width="1145" alt="Note Saved Successfully" src="https://github.com/user-attachments/assets/86e9f0f6-5431-48ab-a938-33812f552e99" />

---

## 📖 Read Note Successfully

<img width="1171" alt="Read Note Successfully" src="https://github.com/user-attachments/assets/8c06d381-5600-4d54-ac07-f8d1e6abc863" />

---

## ☁️ Amazon S3 Bucket

<img width="1909" alt="Amazon S3 Bucket" src="https://github.com/user-attachments/assets/bb3493a8-687d-412b-ad3e-23fdf9c22868" />

---

## ⚡ AWS Lambda Function

<img width="1643" alt="AWS Lambda Function" src="https://github.com/user-attachments/assets/811f7ab4-4e85-4174-ac87-88e1988f3842" />

---

## 📊 CloudWatch Logs

<img width="1595" alt="CloudWatch Logs" src="https://github.com/user-attachments/assets/671c51be-8ab9-41b1-8096-c421adbfb5c6" />

---

# 🔄 Workflow

1. User enters a filename and note content in the web application.
2. The frontend sends a **POST** or **GET** request to **Amazon API Gateway**.
3. API Gateway invokes the **AWS Lambda** function.
4. Lambda processes the request.
5. For **POST**, the note is stored as a text file in **Amazon S3**.
6. For **GET**, Lambda retrieves the requested note from **Amazon S3**.
7. **Amazon CloudWatch** records request logs, execution details, and errors.
8. The API returns the response to the frontend for display.

---

# 📌 API Response

### 📝 Create Note

```json
{
  "message": "Note saved successfully."
}
```

### 📖 Read Note

```json
{
  "filename": "meeting.txt",
  "content": "Prepare AWS presentation."
}
```

---

# 🎯 Learning Outcomes

- Building REST APIs using Amazon API Gateway
- Creating AWS Lambda functions
- Storing and retrieving text files from Amazon S3
- Implementing serverless architecture
- Monitoring and debugging applications with Amazon CloudWatch
- Connecting frontend applications with AWS services
- Working with HTTP GET and POST methods

---

# 🔮 Future Improvements

- ✏️ Edit existing notes
- 🗑️ Delete notes
- 🔍 Search notes by filename
- 🔐 User Authentication using Amazon Cognito
- 🗃️ Store note metadata in Amazon DynamoDB
- 🌙 Dark Mode support
- 📱 Enhanced mobile responsiveness

---

# 👨‍💻 Author

**Mohit Patel**

B.Tech – Artificial Intelligence & Machine Learning

Learning AWS Cloud & Java Development

---

⭐ If you found this project helpful, consider giving it a **Star** on GitHub.
