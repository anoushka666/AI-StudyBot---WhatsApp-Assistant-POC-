# 🤖 **AI StudyBot – WhatsApp Assignment Manager (POC)**

A WhatsApp-based automation system built using **n8n**, **Google Sheets**, and **Twilio**.

This project demonstrates **end-to-end workflow automation**, including webhook handling, intent detection, database operations, and real-time WhatsApp messaging.

---

## 🚀 **Features**

- ✅ **Add assignments** via WhatsApp  
- 📋 **View all assignments**  
- ✔️ **Mark assignments as completed**  
- 📩 **Automatic WhatsApp confirmations**  
- 🤖 **AI-based doubt solving** (optional module)

---

## 🛠 **Tech Stack**

- **n8n** – Workflow automation platform  
- **Google Sheets** – Assignment database  
- **Twilio WhatsApp API** – Messaging integration  
- **OpenAI API** – AI-powered responses (optional)

---

## 📱 **Supported WhatsApp Commands**

### ➕ Add Assignment
```
add <subject> <task> <due_date>
```

### 📋 View Assignments
```
view assignments
```

### ✔️ Mark as Completed
```
done <assignment_number>
```

---

## 🧠 **Workflow Architecture**

```
WhatsApp Message
        ↓
Twilio Webhook
        ↓
n8n Workflow
        ↓
Intent Detection
        ↓
Google Sheets (Add / View / Update)
        ↓
Twilio Response
```

---

## ⚙️ **Setup Instructions**

1. Import the workflow JSON into **n8n**.
2. Create and configure your own credentials:
   - **Google Sheets OAuth2**
   - **Twilio API credentials**
   - **OpenAI API key** (optional)
3. Replace the placeholders:
   - `YOUR_GOOGLE_SHEET_ID`
   - `YOUR_SHEET_NAME`
4. Activate the workflow.
5. Configure Twilio to send WhatsApp webhooks to your **n8n production URL**.

---

## 🔒 **Security Notice**

This repository does **NOT** contain:

- API keys  
- Twilio credentials  
- Google Sheet IDs  
- Production webhook URLs  
- Personal phone numbers  

All credentials must be configured locally in n8n.

---

## 🎯 **What This Project Demonstrates**

- Webhook-based automation  
- Regex-based intent detection  
- Dynamic message parsing  
- Google Sheets as a lightweight database  
- API integrations (Twilio & OpenAI)  
- Secure credential handling practices  

---

## 🚧 **Future Improvements**

- Multi-user support  
- Natural language intent classification  
- Assignment reminders  
- Web dashboard UI  
- Enhanced error handling  

---

## 📌 **Project Status**

**Proof-of-Concept (POC)**

---

## 👩‍💻 Author

Built as a hands-on automation project to explore real-world API integrations and workflow design using n8n.
