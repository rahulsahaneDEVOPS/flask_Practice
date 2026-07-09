# Student Registration System with Jenkins CI/CD

![Project Demo](screenshots/21_Jenkins_Pipeline_SUCCESS.png)

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Flask](https://img.shields.io/badge/Flask-Web%20Application-black?logo=flask)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?logo=mongodb)
![Jenkins](https://img.shields.io/badge/Jenkins-CI%2FCD-red?logo=jenkins)
![Pytest](https://img.shields.io/badge/Pytest-Testing-yellow?logo=pytest)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?logo=github)
![Webhook](https://img.shields.io/badge/GitHub-Webhook-blueviolet)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-orange?logo=ubuntu)
![SMTP](https://img.shields.io/badge/Gmail-SMTP-red?logo=gmail)
![License](https://img.shields.io/badge/License-MIT-blue)

## Project Overview

This project is a **Flask-based Student Registration System** integrated with **MongoDB** for database operations. The application allows users to perform CRUD (Create, Read, Update, Delete) operations on student records.

In addition to the Flask application, this project demonstrates a complete **CI/CD pipeline using Jenkins**, including:

- GitHub Integration
- GitHub Webhook Trigger
- Automated Build
- Automated Testing using Pytest
- Automated Deployment
- Gmail SMTP Email Notification

This project was developed as part of a DevOps learning assignment.

---

# Features

### Student Management

- View Students
- Add Student
- Update Student
- Delete Student

### CI/CD Features

- Jenkins Pipeline
- GitHub Webhook Trigger
- Automated Build
- Automated Pytest Execution
- Automated Deployment
- Gmail SMTP Notification
- Jenkins Console Logs
- Build Status Verification

---

# Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Backend |
| Flask | Web Framework |
| MongoDB | Database |
| HTML | Frontend |
| Bootstrap | UI |
| Jenkins | CI/CD |
| Git | Version Control |
| GitHub | Source Code Repository |
| GitHub Webhook | Auto Trigger Pipeline |
| Pytest | Automated Testing |
| Gmail SMTP | Email Notification |
| ngrok | Public Tunnel |

---

# Project Structure

```
flask_Practice/
│
├── templates/
├── screenshots/
├── app.py
├── Jenkinsfile
├── requirements.txt
├── README.md
└── test_app.py
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/rahulsahaneDEVOPS/flask_Practice.git
```

---

## Move to Project Folder

```bash
cd flask_Practice
```

---

## Create Virtual Environment

Windows

```bash
python -m venv venv
```

Linux

```bash
python3 -m venv venv
```

---

## Activate Virtual Environment

Windows

```bash
venv\Scripts\activate
```

Linux

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Configure Environment Variables

Create a **.env** file

```
MONGO_URI=<Your MongoDB URI>

SECRET_KEY=<Your Secret Key>
```

---

## Run Application

```bash
python app.py
```

Open Browser

```
http://localhost:8000
```

---

# Jenkins CI/CD Pipeline

The Jenkins Pipeline performs the following stages:

- Clone Repository
- Install Dependencies
- Run Pytest
- Deploy Application
- Send Email Notification

Pipeline Stages

```
Checkout Source Code

↓

Install Dependencies

↓

Run Pytest

↓

Deploy

↓

Email Notification
```

---

# GitHub Webhook

GitHub Webhook is configured to automatically trigger Jenkins whenever code is pushed to the GitHub repository.

Workflow:

```
Git Push

↓

GitHub Webhook

↓

Jenkins Pipeline

↓

Build

↓

Testing

↓

Deployment

↓

Email Notification
```

---

# Gmail SMTP Notification

SMTP configuration is integrated with Jenkins.

Whenever a pipeline executes successfully, Jenkins automatically sends an email notification.

---

# Project Screenshots

---
## 1. GitHub Repository

Repository containing the complete Flask project source code.

![GitHub Repository](screenshots/01_GitHub_Repository.png)

---

## 2. Pytest - 4 Tests Passed

All automated test cases executed successfully.

![Pytest 4 Passed](screenshots/02_Pytest_4Passed.png)

---

## 3. Jenkins Dashboard

Jenkins Dashboard showing the configured pipeline.

![Jenkins Dashboard](screenshots/03_Jenkins_Dashboard.png)

---

## 4. Create Jenkins Pipeline

Pipeline creation in Jenkins.

![Create Pipeline](screenshots/04_Create_Pipeline.png)

---

## 5. Pipeline Configuration

Pipeline configuration using Pipeline Script from SCM.

![Pipeline Configuration](screenshots/05_Pipeline_Configuration.png)

---

## 6. Pipeline Trigger Configuration

Trigger configuration for automatic execution.

![Triggers Page](screenshots/06_Triggers_Page.png)

---

## 7. Pipeline from SCM

Pipeline configured to fetch Jenkinsfile from GitHub.

![Pipeline From SCM](screenshots/07_Pipeline_From_SCM.png)

---

## 8. GitHub Repository Connected

GitHub repository successfully connected with Jenkins.

![Repository Connected](screenshots/08_Jenkins_GitHub_Repository_Connected.png)

---

## 9. Jenkins SSH Credential

SSH credentials configured in Jenkins.

![SSH Credential](screenshots/09_Jenkins_SSH_Credential.png)

---

## 10. Initial Build Failed

First build failed before Jenkinsfile was added.

![Build Failed](screenshots/10_Build_Triggered_Failed.png)

---

## 11. Jenkinsfile Missing Error

Pipeline failed because Jenkinsfile was not available.

![Jenkinsfile Missing](screenshots/11_Build_Failed_Jenkinsfile_Missing.png)

---

## 12. Jenkinsfile Verified

Jenkinsfile issue identified and verified.

![Verified Jenkinsfile](screenshots/12_Verified_Jenkinsfile_Missing.png)

---

## 13. Jenkinsfile Created

Jenkinsfile created successfully.

![Jenkinsfile Created](screenshots/13_Jenkinsfile_Created.png)

---

## 14. Jenkinsfile Pushed to GitHub

Updated Jenkinsfile pushed to GitHub repository.

![Jenkinsfile Pushed](screenshots/14_Jenkinsfile_Pushed_GitHub.png)

---
## 15. Fixed Jenkinsfile Syntax

Jenkinsfile syntax corrected successfully.

![Fixed Jenkinsfile Syntax](screenshots/15_Fixed_Jenkinsfile_Syntax.png)

---

## 16. Jenkins Build Success

Build completed successfully.

![Jenkins Build Success](screenshots/16_Jenkins_Build_Success.png)

---

## 17. Jenkins Dashboard After Successful Build

Dashboard showing successful pipeline execution.

![Jenkins Dashboard Success](screenshots/17_Jenkins_Dashboard_Success.png)

---

## 18. GitHub Webhook Created

GitHub webhook configured successfully.

![GitHub Webhook Created](screenshots/18_GitHub_Webhook_Created.png)

---

## 19. Pipeline Started by GitHub Push

Pipeline automatically triggered after GitHub Push.

![Started By GitHub Push](screenshots/19_Started_By_GitHub_Push.png)

---

## 20. Pytest - 4 Tests Passed in Jenkins

All four automated tests passed successfully during Jenkins pipeline execution.

![Pytest Passed](screenshots/20_Pytest_4Passed.png)

---

## 21. Jenkins Pipeline Success

Complete Jenkins pipeline executed successfully.

![Pipeline Success](screenshots/21_Jenkins_Pipeline_SUCCESS.png)

---

## 22. Deployment Success

Application deployed successfully.

![Deployment Success](screenshots/22_Deploy_SUCCESS.png)

---

## 23. Deployment Triggered by GitHub Webhook

Deployment executed automatically after GitHub webhook trigger.

![Deployment Webhook Success](screenshots/23_Deploy_Webhook_SUCCESS.png)

---

## 24. Jenkins Credentials Configuration

Jenkins credentials configured successfully.

![Jenkins Credentials](screenshots/24_Jenkins_Credentials.png)

---

## 25. Google App Password

Google App Password generated for SMTP authentication.

![Google App Password](screenshots/25_Google_App_Password.png)

---

## 26. Gmail SMTP Configuration

SMTP configured successfully in Jenkins.

![SMTP Configuration](screenshots/26_gmail_smtp_configuration.png)

---

## 27. Email Notification Successfully Sent

Jenkins successfully sent email notification after pipeline execution.

![Email Notification](screenshots/27_Email_Test_Successfully_Sent.png)

---

# Project Outcome

The project successfully demonstrates:

- Flask Web Application
- MongoDB Integration
- Jenkins Pipeline
- GitHub Repository Integration
- GitHub Webhook Automation
- Jenkins SSH Authentication
- Automated Build
- Automated Testing using Pytest
- Automated Deployment
- Gmail SMTP Email Notification
- Complete CI/CD Workflow

---

# Author

**Rahul Sahane**

GitHub: https://github.com/rahulsahaneDEVOPS

---

# License

This project is available under the MIT License.
