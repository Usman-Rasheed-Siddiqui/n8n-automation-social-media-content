# n8n-automation-social-media-content
An n8n-based social media automation workflow that validates content, routes approvals, handles errors, and publishes posts to Instagram, Facebook, and LinkedIn with full tracking and user notifications.

> **Note:** This workflow can be run on the [official n8n website](https://n8n.io/)

---

## 📑 Table of Contents
- [Features](#✨-features)
  - [Centralized Social Media Management](#📂-centralized-social-media-management)
  - [Structured Approval Process](#📤-structured-approval-process)
  - [Rule-Based Validation](#⚡-rule-based-validation)
  - [Real-Time Error Feedback](#🛎️-real-time-error-feedback)
  - [Time Efficiency](#⏱️-time-efficiency)
  - [Error Handling & Reliability](#⚠️-error-handling--reliability)
  - [Transparency & Tracking](#📊-transparency--tracking)
  - [Flexible Content Formatting](#✍️-flexible-content-formatting)
- [How the Workflow Works](#🧪-how-the-workflow-works)
  - [1️⃣ User Form Submission](#1️⃣-user-form-submission)
  - [2️⃣ Initial Validation & Classification](#2️⃣-initial-validation--classification)
  - [3️⃣ Approval Routing Logic](#3️⃣-approval-routing-logic)
  - [4️⃣ Admin Approval Stage](#4️⃣-admin-approval-stage)
  - [5️⃣ Social Media Posting](#5️⃣-social-media-posting)
  - [6️⃣ Error Handling & Logging](#6️⃣-error-handling--logging)
  - [7️⃣ Final Status Update & Tracking](#7️⃣-final-status-update--tracking)
- [Future Enhancements](#📦-future-enhancements)
- [Potential Problems](#❗-potential-problems)
- [License](#📘-license)

---

## ✨ Features

### 📂 Centralized Social Media Management
- Manage content posting across multiple platforms from a single workflow.

### 📤 Structured Approval Process
- Reduces risk of unauthorized or incorrect content being published.

### ⚡ Rule-Based Validation
- Automatically enforces official post guidelines (image dimensions, formats, and content rules).

### 🛎️ Real-Time Error Feedback
- Sends email notifications when:
  - Images are private or invalid  
  - URLs are incorrect or not from Google  
  - Other issues occur during the workflow  

### ⏱️ Time Efficiency
- Eliminates manual back-and-forth between content creators and administrators.

### ⚠️ Error Handling & Reliability
- Detects and manages failures gracefully without breaking the workflow.

### 📊 Transparency & Tracking
- Updates Google Sheets with:
  - Form submissions (media link, platform, status, post type)  
  - Event logs (post IDs, success/failure, timestamps)  
- Each post has a unique ID for tracking and updates during the workflow.

### ✍️ Flexible Content Formatting
- Supports:
  - Bullet points  
  - Paragraph-based captions  
  - Platform-specific caption formats  

---

## 🧪 How the Workflow Works

### 1️⃣ User Form Submission
- Users submit a Google Form containing:
  - Post content  
  - Caption text  
  - Platform selection (Instagram, Facebook, LinkedIn)  
  - Post type (Official / Non-Official)  
  - Image or media upload  

### 2️⃣ Initial Validation & Classification
- Checks required fields  
- Determines post type (Official or Non-Official)  
- Validates media links and image dimensions  
- Sends email notifications and updates Google Sheet for errors  

### 3️⃣ Approval Routing Logic
- **Official posts:** Verified against guidelines, then routed for admin review  
- **Non-official posts:** Routed directly for admin review  

### 4️⃣ Admin Approval Stage
- Admin approves or rejects posts  
- Email notifications sent and Google Sheet updated accordingly  

### 5️⃣ Social Media Posting
- Publishes posts to Instagram, Facebook, and LinkedIn  
- Handles caption formatting and media attachment  

### 6️⃣ Error Handling & Logging
- Logs API or media errors  
- Sends detailed notifications to users  
- Updates Google Sheet with failure status  

### 7️⃣ Final Status Update & Tracking
- Google Sheet updated with:
  - Media link, platform, post status  
  - Admin remarks  
  - Publisher status  
  - Event logs (post ID, timestamps)  

---

## 📦 Future Enhancements
- **Multiple Photo Uploads:** Support galleries or carousel posts  
- **Scheduled Posting:** Publish posts at specific dates and times  
- **Comments Management:** Track, moderate, or respond to comments  
- **Mentions Handling:** Detect and process mentions/tags  
- **Enhanced Error Handling:** Advanced checks for multiple images or API limitations  
- **Scalable Reporting:** Extended tracking for scheduled time, images, mentions, and comment actions  

---

## ❗ Potential Problems
- Workflow depends on Google Form and Google Sheets configuration.  
- Social media API limits may affect posting frequency or automation.
- Local Host can raise errors due to limitations

---

## 📘 License
This project is developed solely for educational use and academic evaluation. It is **not intended for commercial deployment or distribution**.
