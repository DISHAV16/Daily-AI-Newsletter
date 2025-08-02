
---

## 📁 **Daily AI Newsletter – README.md**

```markdown
# 📰 Daily AI Tech Newsletter Automation (n8n + OpenAI)

This project automates the creation and delivery of a daily tech newsletter using **n8n workflows** and **GPT-4o**. It fetches the latest news from APIs and RSS feeds, formats them, and emails a summarized version to subscribers.

---

## 🔧 Tools & Platforms Used

- 🧠 OpenAI GPT-4o-mini
- 🔁 n8n (Workflow Automation)
- 📡 NewsAPI & TechCrunch RSS
- 📋 Google Sheets (Data Store)
- 📧 Gmail (Email Sender)

---

## 🔗 Workflow Overview

### Workflow 1 – `Content Collector`
- Trigger: Every 4 hours
- Fetches tech news via:
  - NewsAPI
  - TechCrunch RSS
- Standardizes and stores in Google Sheets

### Workflow 2 – `Newsletter Generator`
- Trigger: Every day at 8 AM
- Reads news from Google Sheets
- Summarizes using OpenAI GPT
- Sends email via Gmail

## 📚 How to Import in n8n

1. Go to your n8n instance.
2. Click “Import” and upload the provided `.json` workflow files.
3. Connect your credentials (API keys for NewsAPI, Gmail, OpenAI).
4. Set your schedule triggers.

---

## 📌 Output

- Daily summarized tech news via email
- Automated and hands-free

---

## 💡 Future Enhancements

- Add topic-based filtering
- Support for WhatsApp/Telegram delivery
- Store email logs
