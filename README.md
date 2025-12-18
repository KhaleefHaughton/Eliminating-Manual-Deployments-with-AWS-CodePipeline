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



