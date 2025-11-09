# Agentic-AI---Resume-Scoring-Agent
An Agentic AI-based HR Automation System that parses resumes, extracts structured candidate information, scores profiles against job requirements, and sends automated follow-up emails. It reduces manual HR work, ensures unbiased screening, and can scale into a SaaS platform for managing multiple hiring pipelines.

# Agentic AI Resume Scoring & HR Automation System

This project is an **Agentic AI-based HR Automation Solution** designed to automate and streamline the recruitment workflow. It intelligently parses resumes, extracts structured candidate information, evaluates profiles using a rule-based scoring engine, updates Google Sheets automatically, and sends scheduled follow-up emails to applicants. This eliminates repetitive manual HR tasks and delivers faster, unbiased, and consistent candidate screening.

The framework is designed to scale into a **full SaaS HR Automation Product**, capable of managing multiple job postings, applicant pipelines, and real-time recruitment workflows.

---

## 🚀 Key Features
- Automatic **Resume Parsing** (PDF/DOCX/Text)
- Extraction of **Skills, Education, Experience, Location, and Tagline**
- **Rule-Based Candidate Scoring** with configurable criteria
- Full integration with **Google Sheets** (Candidate Database + Job Master Data)
- **Automated Follow-Up Email Scheduling** via Gmail/SMTP
- Supports **continuous background execution** using APScheduler
- Modular structure for scaling into **HR SaaS Platform**

---

## 🧠 Technology Stack

| Component | Tools / Libraries Used |
|----------|------------------------|
| Programming Language | **Python 3.12** |
| Resume Parsing | `pdfminer.six`, `python-docx` |
| Data Handling & Processing | `pandas` |
| Sheets & Cloud Data Storage | `gspread`, `Google OAuth Service Account` |
| AI / Rule-Based Scoring | Custom Scoring Engine (configurable JSON rules) |
| Notifications / Emails | `smtplib` / Gmail API |
| Task Scheduling | `APScheduler` |
| Environment Config | `python-dotenv` |
| Optional Dashboard (Future Extension) | `Streamlit` |

---

## 🗂 Data Flow Overview

Candidate Resume
↓
Resume Parser → Extracted Data
↓
Candidate Scoring Engine → Score Assigned
↓
Google Sheets Updated with Results
↓
Automated Follow-Up Emails Sent

yaml
Copy code

---

## 🔧 Setup Instructions

### 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt

2️⃣ Configure Environment Variables in .env
ini
Copy code
GOOGLE_SERVICE_ACCOUNT_JSON=service_account.json
MASTER_SHEET_ID=your_master_sheet_id
DETAIL_SHEET_ID=your_detail_sheet_id
SMTP_USER=your_gmail_address
SMTP_PASSWORD=your_app_password   # Gmail App Password
FROM_EMAIL=your_gmail_address

3️⃣ Run the Script One Time
bash
Copy code
python resume_parser_agent.py --run-once

4️⃣ Run Automation Continuously in Background
bash
Copy code
python resume_parser_agent.py --schedule
📌 Example Use Case
Field	Example Value
Education	B.Tech 2025
Location	Hyderabad
Internship Experience	6+ Months
Score Assigned	75 / 100
Follow-Up Status	Auto-Email Sent

🛠 Future Enhancements
AI/LLM-based semantic candidate-job matching

Multi-job recruitment pipeline dashboard

LinkedIn / WhatsApp outreach automation

HR analytics reporting dashboard

🏁 Conclusion
This system replaces repetitive manual HR screening steps with intelligent automation, improving speed, fairness, and efficiency. It is ideal for Companies, HR Teams, Startups, Placement Offices, and SaaS Recruiter Platforms.

⭐ If you find this project useful, please star the repo!
yaml
Copy code

---

If you want, I can now:

✅ Add **Badges** (Python, License, Stars, etc.)  
✅ Add **Flowchart Diagram**  
✅ Add **Screenshot Preview UI**  
✅ Generate **GitHub Repository Banner**
