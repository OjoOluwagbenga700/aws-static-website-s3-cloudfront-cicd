# 🚀 Host a Static Website on AWS S3 + CloudFront with Github Action CI/CD (ClickOps)

A beginner-friendly project to host a static website using:
- Amazon S3 (for storage)
- Amazon CloudFront (for global delivery)
- GitHub Actions (for auto deployment)

## 🛠️ Prerequisites

✅ AWS Account  
✅ GitHub Repository  
✅ Basic HTML/CSS files

## 🖱️ Step 1: Create Your S3 Bucket (via AWS Console)
1. Go to **S3 > Create Bucket**
2. Name: `your-static-site-name`
3. Uncheck "Block all public access"
4. Enable **static website hosting**
5. Upload your site manually to test

## 🌐 Step 2: Add CloudFront (Optional)
1. Go to **CloudFront > Create Distribution**
2. Origin: your S3 bucket website endpoint
3. Enable caching, add custom domain (optional)
4. Note the **Distribution ID**

## 🔐 Step 3: Setup GitHub Secrets

| Name                 | Description               |
|----------------------|---------------------------|
| `AWS_ACCESS_KEY_ID`  | Your IAM Access Key       |
| `AWS_SECRET_ACCESS_KEY` | Your IAM Secret Key |
| `S3_BUCKET_NAME`     | Your S3 bucket name       |
| `CLOUDFRONT_ID`      | Your CloudFront Dist. ID  |

## 🤖 Step 4: GitHub Actions CI/CD Pipeline

Refer to `.github/workflows/deploy.yml` to automate S3 sync and CloudFront cache invalidation.

## 🧠 What You’ll Learn
- How to host websites using S3 + CloudFront manually (ClickOps)
- Set up GitHub Actions for automatic deployment
- Secure static hosting with cache invalidation


# aws-static-website-s3-cloudfront-github-cicd
