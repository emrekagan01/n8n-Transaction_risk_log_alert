# 🚨 Real-Time Transaction Risk Monitoring (n8n)

## 📌 Overview
This project implements a real-time transaction risk monitoring pipeline using **n8n**.  
Incoming transaction data is evaluated against predefined risk rules, enriched with AI-based analysis, logged for auditing, and triggers automated alerts when anomalies are detected.

The workflow simulates a production-ready event-driven architecture for financial risk monitoring systems.

---

## 🎯 Problem
In financial systems, high-value or suspicious transactions must be detected **immediately** to prevent fraud, ensure compliance, and enable rapid response.

Manual monitoring is:
- Slow
- Error-prone
- Not scalable

---

## 💡 Solution
This workflow automates the entire process:

- Receives transactions in real time via webhook
- Applies rule-based risk detection
- Enriches results with AI-based reasoning (simulated)
- Logs results for audit and traceability
- Sends automated alerts for high-risk cases

---

## ⚙️ Architecture

Webhook → Data Normalization → Risk Detection → AI Analysis → Formatting → Logging → Alert

---

## 🔍 Key Features

- ⚡ Real-time processing via webhook
- 📊 Threshold-based risk detection
- 🤖 AI-based risk enrichment (demo placeholder)
- 🧾 Audit logging via Google Sheets
- 📩 Automated alerting via email
- 🔒 Security-first design (sanitized for public sharing)

---

## 📥 Example Input

```json
{
  "transaction_id": "TX1001",
  "amount": 15000,
  "currency": "USD",
  "description": "High-value transfer"
}
```

---

## 📤 Example Output (Risk Evaluation)

```json
{
  "risk_level": "high",
  "short_reason": "High transaction amount",
  "recommended_action": "manual_review"
}
```

---

## 🚨 Alert Example

When a high-risk transaction is detected, an alert is generated containing:

- Transaction ID
- Amount & Currency
- Risk Level
- Reason
- Recommended Action

---

## 🧪 How to Use

1. Import `workflow.json` into n8n
2. Configure your own credentials:
   - Email (SMTP or Gmail)
   - Google Sheets (optional)
3. Trigger the webhook using `sample_payload.json`
4. Observe:
   - Risk detection
   - Logging
   - Alert triggering

---

## 🔐 Security Notice

This repository contains a **sanitized version** of the workflow:

- No API keys
- No real email addresses
- No production endpoints
- No real database connections

All external integrations are replaced with placeholders.

---

## 🛠 Tech Stack

- n8n (workflow automation)
- Webhooks (event ingestion)
- Google Sheets (logging)
- Email (alerting)
- AI API (simulated)

---

## 👤 Author

Built as part of a transition into Data Engineering / AI Engineering roles, focusing on real-world automation and event-driven systems.
