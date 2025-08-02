# 📩 n8n-Email-Agent-Automationx
<img width="1878" height="1140" alt="2- Mail Flow - summed" src="https://github.com/user-attachments/assets/f890e303-7a8e-42af-a1e2-6ac8201f82a9" />

A fully automated email processing workflow built with [n8n](https://n8n.io).
This agent is designed to help you organize incoming emails past, present, and future based entirely on your custom rules and preferences.

## ⚙️ Overview

This project automates the handling of your Gmail inbox using a modular and scalable n8n workflow. It integrates with **Gmail**, **AWS S3**, **MongoDB**, and **Google Sheets** to automatically filter, extract, store, and structure email data eliminating the need for manual filtering, downloading, and data entry.

---

## 🔧 Features

### ✅ Automated Email Trigger

* Reacts in real-time when a new email arrives.
* Ensures immediate data capture and processing.

### 🔍 Dynamic Filtering

* Filters emails based on:

  * Sender email
  * Subject line or body keywords
  * Attachment presence and file metadata

### 📨 Metadata Extraction

* Extracts all relevant email metadata including:

  * Sender, recipients, subject, timestamps, headers, etc.

### 🔗 URL Extraction

* Uses regex-based logic to scan and extract all URLs from the email body.

### 📎 Attachment Handling

* Detects and extracts file names and binary data from email attachments.
* Prepares attachments for further actions.

### ☁️ AWS S3 Integration

* Uploads attachments directly to an S3 bucket.
* Uses safe, dynamic naming to avoid overwrite or collisions.

### 🧮 MongoDB Integration

* Maps extracted content and performs upserts into a MongoDB collection.
* Enables structured storage for later querying and analysis.

### 📊 Google Sheets Configuration

* Dynamically fetches filtering and extraction rules from a Google Sheet.
* Allows non-technical users to modify behavior without editing the workflow.

### 🧱 Modular, Scalable Design

* Each email is processed independently.
* Supports high-volume inboxes without performance degradation.

### 💻 Custom JavaScript Logic

* Fine-grained data mapping and validation using Code Nodes.
* Ensures high accuracy and flexible workflow control.

---

## 📁 Technologies Used

* [n8n](https://n8n.io/)
* Gmail API
* AWS S3
* MongoDB
* Google Sheets API
* JavaScript (Code Nodes)

---

## 📌 Use Cases

* Automate archiving of important attachments to cloud storage
* Build a searchable database of emails and related files
* Filter and track specific types of emails (e.g., invoices, reports, links)
* Reduce manual workload for operations or customer support teams
