# Assignment 1 — AWS Free Tier Account Setup (EpicReads Cloud Onboarding)

Part of the DevOps Micro Internship (DMI) with Agentic AI

---

## Purpose

In this assignment, you will create and verify an AWS Free Tier account as part of onboarding EpicReads — an online bookstore moving to the cloud. You will demonstrate an understanding of AWS fundamentals, Free Tier services, and account setup by answering conceptual questions and capturing proof of a working AWS Console login.

---

# Task 1 — Understanding AWS & Free Tier

## Goal

Demonstrate understanding of AWS basics and Free Tier usage by answering the following questions in your own words (3–4 lines each).

### Answers

#### Question 1 — What is an AWS account, and why do you need it at this stage?

An AWS account is your personal or organization account used to access Amazon Web Services (AWS) cloud services.
At this stage of your DevOps Micro Internship, you need an AWS account because your project uses AWS infrastructure:
- Amazon S3 – to store and host your static website files.
- CloudFront – to deliver the website quickly through a CDN.
- Terraform – to create and manage these AWS resources automatically.
- GitHub Actions – to automate deployment to AWS.
Simple example
Your workflow will look like:
Code → GitHub → GitHub Actions → Terraform → AWS S3 + CloudFront → Website
So, the AWS account provides the cloud environment where your DevOps project will actually be deployed and tested.

---

#### Question 2 — What is AWS Free Tier, and how long does it last?

As of October 2026, AWS offers a new-account Free account plan for up to 6 months, or until your free credits are used up, whichever comes first. AWS Documentation
Here's what you get:
- $100 in AWS credits when you create a new account.
- An opportunity to earn up to an additional $100 in credits by completing eligible activities.
- Access to more than 30 services with ongoing free usage allowances, subject to individual limits. Amazon Web Services, Inc.
💻 How does this help your DevOps internship?
For your project, you plan to use:
- Amazon S3 — to host your static website.
- Amazon CloudFront — to deliver your website to visitors.
- Terraform — to automate AWS infrastructure creation.
You can explore AWS and deploy your project, but check the pricing and free-plan eligibility of each service before using it.
⚠️ Important things to remember
1. The Free account plan ends after six months or when your credits run out.
2. After the Free plan expires, your account closes unless you upgrade within the applicable recovery period.
3. Some services have separate free usage limits, and those limits may continue after the six-month period.
4. Monitor your credit balance and usage to avoid unexpected costs if you upgrade to a paid plan.

---

#### Question 3 — Name three AWS Free Tier services and their free usage limits.

Amazon EC2: Provides free usage for eligible virtual server instances within the applicable plan limits.
Amazon S3: Offers free storage for eligible usage within the applicable monthly limits.
AWS Lambda: Offers a free monthly allowance of 1 million requests and 400,000 GB-seconds of compute time under its eligible free usage allowance

---

# Task 2 — Create AWS Free Tier Account

## Goal

Create a valid AWS Free Tier account and sign in to the AWS Management Console.

> No screenshots required for this task. Completion is verified through Task 3.

---

# Task 3 — Verify AWS Account

## Goal

Confirm that your AWS account setup is complete by navigating to the Account section and capturing proof.

### Evidence

#### Screenshot 1 — AWS Account page showing account name (email may be blurred)

Add your screenshot here.

---


# Submission Instructions

- Add all required screenshots in your GitHub repository submission
- Full name must be visible in required screenshots
- Do not expose sensitive information (keys, passwords, account IDs)
- Share your AWS onboarding progress on WhatsApp Status (Task 4)

---

# Completion Checklist

- [✅] Task 1 answers written in own words
- [✅] AWS Free Tier account created successfully
- [✅] Signed in to AWS Management Console
- [✅] Screenshot 1 of AWS Account page captured (full name visible, no sensitive data)
- [✅] Task 4: AWS onboarding progress shared on WhatsApp Status
- [✅] Screenshot 2 of published WhatsApp Status captured with leaderboard progress link visible
- [✅] All required screenshots added to repository

---

## 📌 About DMI & CloudAdvisory

DevOps Micro Internship (DMI) is a project-based DevOps program run by Pravin Mishra (The CloudAdvisory) focused on real-world execution, systems thinking, and career readiness.

It helps learners build strong DevOps foundations with hands-on experience.

---

## 📌 Resources

- 🌐 DMI Official Website: https://dmi.pravinmishra.com?utm_source=github&utm_medium=readme  
- 🎓 University: https://university.pravinmishra.com?utm_source=github&utm_medium=readme  
- 💬 Discord Community: https://discord.pravinmishra.com?utm_source=github&utm_medium=readme  
- 📝 Blog: https://dmi.pravinmishra.com/blog?utm_source=github&utm_medium=readme  
- ▶️ YouTube Playlist: https://www.youtube.com/playlist?list=PLFeSNDtI4Cho  
- 🔗 Pravin Mishra (LinkedIn): https://www.linkedin.com/in/pravin-mishra-aws-trainer/  
- 🏢 CloudAdvisory (LinkedIn): https://www.linkedin.com/company/thecloudadvisory/

---

*This submission is part of DevOps Micro Internship (DMI) — Agentic AI Track.*
