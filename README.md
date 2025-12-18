# Eliminating-Manual-Deployments-with-AWS-CodePipeline
Seamless Web Delivery: CI/CD Pipeline with AWS CodePipeline &amp; S3

# AWS Static Website CI/CD with CodePipeline & S3

This repository contains a **static website** and documentation to automatically deploy it using **AWS CodePipeline** into an **Amazon S3 bucket** that hosts a static site.


---

## 🚀 What This Project Does

- 🎯 Hosts a static website in an AWS S3 bucket enabled for static website hosting
- 🔁 Uses AWS CodePipeline to automatically deploy changes from GitHub to S3
- 📈 Enables continuous deployment — every update is published live
- 💡 Uses only AWS managed services — no servers required

---

## 🧱 Project Structure

aws-static-website-cicd/
├── website/
│ ├── index.html
│ ├── styles.css
│ └── assets/
│ └── logo.png
├── .github/
│ └── workflows/
│ └── github-ci.yml # OPTIONAL GitHub Actions CI/CD pipeline
├── .gitignore
└── README.md

## 1. Configure AWS CodePipeline

Go to the AWS Console → CodePipeline.

Create a new pipeline.

Choose GitHub as the provider.

Connect to your repository and pick your default branch.

Skip the build stage — static HTML doesn’t need a build.

For Deploy, choose Amazon S3 and point it to your static bucket.

Review and create the pipeline.

## 2. 🧠 Test Deployment

Visit your S3 bucket’s static website endpoint.

Update index.html (for example, change text).

Commit and push to GitHub.

CodePipeline should trigger and deploy the changes automatically within a few minutes.


## 📂 Static Website Files

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Hello Level Up In Tech!</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h3>Anyone can transition to DevOps. The Steps are:</h3>
    <h3>1. Trust the process</h3>
    <h3>2. Work hard</h3>
    <h3>3. Be consistent</h3>
    <h3>4. Stay Hungry</h3>
    <p>This website is deployed automatically via AWS CodePipeline & S3.</p>
</body>
</html>


