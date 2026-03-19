# 🚀 Serverless Image Processor (AWS)

## 🖼️ Project Image
![Serverless Image Processor](./ChatGPT%20Image%20Mar%2019,%202026,%2012_07_53%20PM.png)

## 📌 Overview
This project demonstrates a serverless image processing pipeline using AWS services.

When an image is uploaded to S3:
- Lambda function is triggered
- Image is processed (copied/resized)
- Metadata stored in DynamoDB
- Notification sent via SNS

---

## 🏗️ Architecture

S3 (Input Bucket)
   ↓
Lambda (Node.js)
   ↓
├── S3 (Output Bucket)
├── DynamoDB (Metadata)
└── SNS (Notification)

---

## ⚙️ AWS Services Used

- Amazon S3
- AWS Lambda
- Amazon DynamoDB
- Amazon SNS
- CloudWatch

---

## 🔄 Workflow

1. Upload image to S3 input bucket
2. S3 triggers Lambda
3. Lambda processes image
4. Stores result in output bucket
5. Saves metadata in DynamoDB
6. Sends notification via SNS

---

## 📦 Features

- Event-driven architecture
- Serverless (no server management)
- Scalable and cost-efficient
- Real-world use case (image processing)

---

## 🧪 How to Run

1. Upload image to S3 input bucket
2. Check output bucket for processed image
3. Check DynamoDB for metadata
4. Check email for notification

---

## 🚀 Future Improvements

- Add image resizing using Sharp
- API Gateway for uploads
- User authentication with Cognito
- CloudFront for CDN

---

## 👨‍💻 Author
Justus Faby Jeyakumar