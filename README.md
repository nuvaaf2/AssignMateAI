<div align="center">

# 🤖 AssignMate AI

### AI-Powered Assignment Tracking & Submission Automation System

[![n8n](https://img.shields.io/badge/Built%20with-n8n-FF6D00?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Gmail](https://img.shields.io/badge/Gmail-IMAP%2FSMTP-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](https://gmail.com)

*Automatically monitors student assignment submissions via email — validates content, checks compliance, and sends smart AI feedback. Zero manual grading.*

</div>

---

## 📌 Overview

AssignMate AI is a fully automated assignment management pipeline built with **n8n** and **OpenAI GPT-4**. When a student submits an assignment via email (PDF or DOC), the system automatically reads the attachment, validates it against academic requirements, and replies with intelligent, personalized feedback — all without any human intervention.

---

## ✨ Features

- 📥 **Email Monitoring** — Continuously watches a dedicated inbox via IMAP for new student submissions
- 📎 **Attachment Parsing** — Extracts and reads PDF/DOC content from email attachments
- 🧠 **AI Content Validation** — GPT-4 checks for academic compliance: topic relevance, formatting, completeness
- 📤 **Smart Feedback Replies** — Sends personalized feedback emails via SMTP with specific improvement suggestions
- ⚠️ **Edge Case Handling** — Detects missing attachments, invalid file types, late submissions, and duplicate entries
- 🔁 **Fully Automated** — Runs 24/7 with no manual input required

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation engine |
| **OpenAI GPT-4** | AI content validation & feedback generation |
| **IMAP** | Incoming email monitoring |
| **SMTP** | Outgoing feedback email delivery |
| **Gmail API** | Email integration |

---

## 🔄 How It Works

```
Student sends email with PDF/DOC attachment
        ↓
n8n detects new email via IMAP trigger
        ↓
Attachment is extracted and parsed
        ↓
GPT-4 validates content & academic compliance
        ↓
AI generates personalized feedback
        ↓
Feedback sent back to student via SMTP email
```

---

## 🚀 How to Use

### Prerequisites
- [n8n](https://n8n.io) (self-hosted or cloud)
- OpenAI API key
- Gmail account with IMAP enabled

### Setup Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/nuvaaf2/assignmate-ai.git
   cd assignmate-ai
   ```

2. **Import the workflow**
   - Open your n8n instance
   - Go to **Workflows → Import from file**
   - Select `assignmate-ai-workflow.json`

3. **Configure credentials**
   - Add your **OpenAI API key** in n8n credentials
   - Set up **Gmail IMAP** credentials (enable IMAP in Gmail settings)
   - Set up **Gmail SMTP** credentials for sending replies

4. **Activate the workflow**
   - Toggle the workflow to **Active**
   - Test by sending a sample assignment email with a PDF attachment

---

## 📂 Repository Structure

```
assignmate-ai/
├── assignmate-ai-workflow.json   # n8n workflow export
```

---

## 📸 Workflow Preview

<img width="1509" height="641" alt="image" src="https://github.com/user-attachments/assets/897834e7-22c0-4656-83d3-c2f9d7ee4203" />


---

## 🔮 Future Improvements

- [ ] Google Classroom integration
- [ ] Plagiarism detection layer
- [ ] Dashboard for teachers to view submission stats
- [ ] Support for ZIP file submissions

---

## 👤 Author

**Nuvaaf A N** — AI Automation Engineer | n8n Builder

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/YOUR_LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-nuvaaf2-181717?style=flat&logo=github)](https://github.com/nuvaaf2)

---

<div align="center">
⭐ If you found this useful, please star the repo!
</div>
