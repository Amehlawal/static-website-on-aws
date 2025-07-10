# 🚀 Static Website Deployment on AWS with GitHub Actions

This project deploys a static HTML/CSS website to Amazon S3 and serves it via CloudFront using GitHub Actions and CloudFormation.

## 📦 Features

- S3 for static file hosting
- CloudFront for secure, fast global delivery
- CloudFormation for infrastructure as code
- GitHub Actions for CI/CD automation
- No custom domain required

---

## 📁 Folder Structure

| Path                    | Description                          |
|-------------------------|--------------------------------------|
| `cfn/static-website.yaml` | CloudFormation infrastructure template |
| `website/`              | Your static website (HTML, CSS, JS) |
| `.github/workflows/`    | CI/CD GitHub Actions workflow        |

---

## 🔧 Prerequisites

- AWS account
- IAM user with S3, CloudFront, and CloudFormation permissions
- GitHub secrets configured:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_REGION` (e.g., `us-east-1`)

---

## 🚀 Deploy Instructions

### 1. Fork this repo

```bash
git clone https://github.com/your-username/static-website-deploy.git
cd static-website-deploy
