# Rainy Day Relics 🌧️

Welcome to the official repository for **Rainy Day Relics**, a static website hosted on AWS and deployed via GitHub Actions.

🔗 [rainydayrelics.com](https://rainydayrelics.com)

---

## 🔭 Overview

Welcome to the official repository for **Rainy Day Relics**, a tabletop role-playing game (TTRPG) and game accessory company. Our website is hosted on AWS and continuously deployed with GitHub Actions.
- **Static Website Hosting:** Amazon S3
- **Continuous Deployment (CI/CD):** GitHub Actions
- **DNS Management:** Amazon Route 53

---

## 🛠️ Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **Hosting:** AWS S3 Bucket
- **Deployment Automation:** GitHub Actions
- **DNS Provider:** AWS Route 53

---

## 📁 Repository Structure

```text
rainydayrelics/
├── .github/
│   └── workflows/        # GitHub Actions workflow definitions
├── public/               # Static files (HTML, CSS, JS, images)
├── src/                  # Source code (optional if using build tools)
└── README.md             # This documentation
```

---

## ⚙️ GitHub Actions CI/CD

The website deploys automatically upon committing or merging to the `main` branch.

### 🔄 Deployment Process:
- Push to `main` branch triggers automatic build and upload.
- Static files sync directly to AWS S3.

### 🔐 Required GitHub Secrets:
Ensure these secrets are configured in your repository (`Settings → Secrets and Variables → Actions`):

| Secret Name             | Description                           |
|-------------------------|---------------------------------------|
| `AWS_ACCESS_KEY_ID`     | AWS IAM Access Key                    |
| `AWS_SECRET_ACCESS_KEY` | AWS IAM Secret Key                    |
| `AWS_REGION`            | AWS region (e.g., `us-west-2`)        |
| `AWS_S3_BUCKET`         | S3 bucket name                        |

---

## 📌 Manual Deployment

To trigger deployment manually:

```bash
git push origin main

