# 🚀 GrowthPath AI-Powered Lead Generation & Qualification System

> **Novara Cohort Capstone Project** — AI & Automation  
> **Client:** GrowthPath Digital Consulting, Lagos, Nigeria

---

## 📌 Project Overview

GrowthPath Digital Consulting receives 80–150 leads per week from multiple channels — website, Instagram, WhatsApp, Facebook, and referrals — with no centralized system to track, qualify, or follow up with them.

This project delivers a **fully automated, AI-powered lead generation and qualification system** that:

- Engages leads instantly across multiple channels (24/7)
- Asks qualifying questions and scores leads as **Hot / Warm / Cold**
- Books meetings on Google Calendar for hot leads automatically
- Logs all lead data into a CRM (Airtable / Google Sheets)
- Sends automated email follow-up sequences via Zapier
- Notifies the sales team in real time via Slack or Email

---

## 🏗️ System Architecture

```
Lead Inquiry (Website / Instagram / WhatsApp / Facebook)
        │
        ▼
 ┌─────────────────┐
 │   AI Chat Agent  │  ← Voiceflow / Chatbase / ManyChat
 │  (Qualification) │
 └────────┬────────┘
          │ Webhook
          ▼
 ┌─────────────────┐
 │  n8n Automation  │  ← Core workflow engine
 │    Workflow      │
 └──┬──────┬───────┘
    │      │
    ▼      ▼
 CRM    Lead Score
 (Airtable/Sheets)
    │
    ├── 🔥 HOT  → Google Calendar Booking + Slack Notification
    ├── 🌡️ WARM → Email Follow-up Sequence (Zapier)
    └── 🧊 COLD → Nurture List + Email Drip
```

---

## 🛠️ Tech Stack

| Component | Tool |
|---|---|
| AI Chat Agent | Voiceflow / Chatbase / n8n AI Agent / ManyChat |
| AI Voice Agent *(Bonus)* | Vapi / Retell AI |
| Messaging Channels | Telegram, WhatsApp, Instagram, Facebook |
| Workflow Automation | n8n |
| CRM / Database | Airtable or Google Sheets |
| Calendar | Google Calendar |
| Email Campaign | Zapier |
| Team Notifications | Slack or Email |
| Landing Page *(Bonus)* | Bolt.new / Lovable |

---

## 📁 Repository Structure

```
growthpath-ai-lead-system/
│
├── 01_AI_Agent/              # Agent configuration, flows, prompts
├── 02_n8n_Workflow/          # n8n workflow JSON exports
├── 03_CRM_Database/          # Airtable schema / Google Sheets templates
├── 04_Calendar_Integration/  # Calendar setup & configuration notes
├── 05_Email_Campaign/        # Zapier workflow + email templates
├── 06_Bonus_Features/
│   ├── AI_Email_Agent/       # AI email responder setup
│   └── Landing_Page/         # Landing page code (Bolt.new / Lovable)
├── 07_Screenshots/           # All required submission screenshots
├── docs/                     # Additional documentation & notes
├── .gitignore
├── LICENSE
└── README.md
```

---

## ✅ Core Features

- [x] AI agent greets and qualifies leads via natural conversation
- [x] Collects: name, email, phone, company, services, budget, timeline
- [x] Automatic lead scoring (Hot / Warm / Cold)
- [x] Lead data pushed to CRM automatically
- [x] Google Calendar booking for Hot leads
- [x] Automated email follow-up campaign (3-email sequence)
- [x] Sales team Slack/email notification for high-value leads

## 🌟 Bonus Features

- [ ] Multi-channel support (Instagram + Telegram)
- [ ] AI email response agent
- [ ] Voice agent (Vapi / Retell AI)
- [ ] Landing page with embedded chatbot
- [ ] Custom CRM views and dashboards
- [ ] Creative weighted lead scoring logic
- [ ] n8n error handling & fallback actions

---

## 📸 Submission Screenshots

All screenshots are stored in `/07_Screenshots/` and labelled as follows:

| File | Description |
| --- | --- |
| [01] CRM(airtable).jpeg | Airtable/Sheets with 3+ test leads |
| [02] error_workflow.jpeg | error workflow should incase of error in the main workflow |
| [03] telegram_hot_lead.jpeg | screenshot of telegram test |
| [04] voiceflow_workflow.jpeg | chat bot workflow |
| [05] website_cold_lead.jpeg | screenshot of website with cold lead |
| [06] website_hot_lead.jpeg | screenshot of website test with hot lead |
| [07] website_warm_lead.jpeg | screenshot of website test with warm lad |
| [08] workflow_outputs.jpeg | screenshot showing each node of the n8n workflow |
| [10] Zapier_workflow.jpeg | Zapier workflow |

---

## 🔗 Live Agent Links

| Platform | Link / Handle |
| --- | --- |
| Voiceflow | [Voiceflow](https://creator.voiceflow.com/share/699925ac603f17b83b30b77d/production ) |
| Telegram | [Grow_Path_TG](https://t.me/Grow_Path_TG_bot) |
| Landing Page | [Lovable](https://growthpath-consulting.lovable.app/) |

---

## 🚀 How to Run / Test the System

1. **Test the AI Agent** — Use the live link above to simulate a lead inquiry
2. **Trigger the n8n Workflow** — The agent sends lead data via webhook to n8n
3. **Check the CRM** — Verify lead data appears in Airtable/Google Sheets
4. **Check Google Calendar** — Confirm appointment was booked for Hot leads
5. **Check Email Inbox** — Confirm the 3-email follow-up sequence triggered
6. **Check Slack** — Confirm the sales team was notified

---

## 👤 Author

**Adeniran Precious Adebayo**  
Novara Cohort — AI & Automation Capstone Project  
[adeniranprecious002@gmail.com](mailto:adeniranprecious002@gmail.com) | [LinkedIn](https://www.linkedin.com/in/precious-adeniran-842b58294)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
