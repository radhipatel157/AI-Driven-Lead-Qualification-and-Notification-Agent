# AI-Driven Lead Qualification and Notification Agent

Automated lead classification and notification system powered by n8n workflows, Google Gemini, and Gmail API.

## Overview

This system processes over 500 form submissions weekly, scoring and qualifying leads using AI via Google Gemini, and auto-notifying stakeholders through intelligent routing.

## Features

- **Form Integration**: Captures submissions via HTTP request triggered by form activity.
- **AI-Based Scoring**: Utilizes Google Gemini for message analysis and lead qualification.
- **Dynamic Routing**: Routes qualified leads to the appropriate team based on classification.
- **Instant Notifications**: Sends real-time email alerts using the Gmail API.
- **Modular Workflows**: Decoupled into classification and notification flows for scalability.

## Workflow Breakdown

### 1. Lead Qualification Agent (Form Submissions)
- Trigger: On form submission
- Sends data via HTTP request
- Processed by the AI Agent (Google Gemini)
- Tools used:
  - Google Gemini (for lead scoring)
  - Call another n8n workflow (for classification and notification)
  - Gmail (to send scored lead emails)

### 2. Qualified Lead Classifier AND Notifier
- Triggered by the first workflow
- Uses Google Gemini to evaluate lead details
- Decision logic (`IF` node) checks the type of lead
- Sends Gmail notifications based on the classification

## Stack

- **n8n**: Workflow automation
- **Google Gemini**: AI model for lead scoring and classification
- **Gmail API**: For sending automated notifications

## Impact

- **500+ leads/week** processed with minimal manual effort
- **80% reduction** in lead triage time
- **Stakeholder response time reduced from 1 hour to 12 minutes**


