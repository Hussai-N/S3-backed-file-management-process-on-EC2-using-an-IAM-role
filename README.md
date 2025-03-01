# S3-backed-file-management-process-on-EC2-using-an-IAM-role

## 📌 Project Overview
This project demonstrates how to configure an **EC2 instance** to manage files stored in an **S3 bucket**, using an **IAM role** for secure access.

## 🚀 Process Flow
1. Launch EC2 Instance.
2. Create an S3 Bucket.
3. Create and attach an **IAM Role** with **S3 permissions** to the EC2 instance.
4. Install AWS CLI on EC2.
5. Use AWS CLI commands to **upload, download, and list files** from S3.

## ⚙️ Technologies Used
- **EC2 (Amazon Elastic Compute Cloud)**
- **S3 (Simple Storage Service)**
- **IAM Role**
- **AWS CLI**

## ✨ Key Benefits
- No hard-coded credentials.
- Secure and scalable.
- Simple automation with shell scripts.

## 📂 Example Commands
```bash
# Upload a file to S3
aws s3 cp /path/to/local/file.txt s3://your-bucket-name/

# Download a file from S3
aws s3 cp s3://your-bucket-name/file.txt /path/to/local/

# List files in the bucket
aws s3 ls s3://your-bucket-name/
