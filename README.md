# 🚀 AI-Driven Lead Qualification & Notification Agent

A fully automated system that classifies, scores, and routes **500+ leads weekly** using AI workflows powered by **n8n**, **Google Gemini**, and the **Gmail API**.

---

## ✨ Overview

Harness the power of AI to streamline your lead management process. This system automates the entire lifecycle — from form submission to stakeholder notification — reducing manual triage by **80%** and improving response times by **5×**.

---

## 🔧 Key Features

- ✅ **Real-Time Form Integration**  
  Instantly captures form submissions via HTTP trigger in n8n.

- 🧠 **AI-Powered Lead Scoring**  
  Leverages Google Gemini to assess and qualify leads intelligently.

- 🔀 **Smart Routing & Classification**  
  Routes high-quality leads to the right teams using dynamic workflows.

- 📩 **Instant Notifications**  
  Sends personalized emails to stakeholders using the Gmail API.

- 🧩 **Modular & Scalable Workflows**  
  Separated into classification and notification pipelines for flexibility and easy updates.

---

## 🛠️ Workflow Architecture

### 📥 1. Lead Qualification Agent
**Trigger**: Form submission via HTTP node  
**Actions**:
- Extract lead details  
- Score message using Google Gemini  
- Invoke downstream workflow for classification + routing

### 📤 2. Lead Classifier & Notifier
**Trigger**: Workflow call from the Qualification Agent  
**Steps**:
- Analyze lead intent and quality with Google Gemini  
- Apply classification logic (`IF` / `SWITCH`)  
- Notify relevant stakeholders using Gmail

---

## 🧱 Tech Stack

| Tool           | Purpose                             |
|----------------|-------------------------------------|
| 🧩 **n8n**      | Workflow automation engine          |
| 🤖 **Gemini**   | AI-based message classification     |
| 📧 **Gmail API**| Sends automated email alerts        |

---

## 📈 Results

- 📊 **500+ leads/week** processed autonomously  
- ⏱️ **80% reduction** in triage time  
- ⚡ **Response time cut from 1 hour → 12 minutes**

---

## 🏗️ Ideal For

- Lead-heavy organizations  
- Sales enablement and CRM workflows  
- Agencies managing multiple intake channels  
- Teams looking to scale without hiring

---

