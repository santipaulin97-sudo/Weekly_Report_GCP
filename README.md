🤖 Automated Supply Chain Monitoring • BigQuery Analytics • Financial Auditing • Logistics KPIs
This repository contains a fully automated Logistics & Financial Monitoring System built in n8n

BigQuery Data Extraction (7 parallel analysis streams)
Financial Estimation (Cost mapping per service code)
Exception Translation (Chinese to Spanish error interpretation)
Python Data Processing (KPI calculation & HTML generation)
Automated Executive Reporting (Rich HTML emails)

✨ Key Features
⏰ 1. Bi-Weekly Automated Schedule
Cron Trigger: Runs automatically every 2 weeks (Mondays at 08:00 AM).

Goal: Detects anomalies and trends before the monthly billing closure.

📊 2. Deep Data Analytics (BigQuery)
The workflow executes 7 parallel SQL queries against meli-bi-data to extract granular insights:

Noise vs. Reality: Filters valid callbacks vs. system noise.
Weekly Trends: Compares volume variations (WoW) to detect spikes.
Daily Control Board: Tracks unique orders vs. total events.

🐍 Python Data Processing 
A custom Python node aggregates the 7 data streams to:
Calculate Month-over-Month (MoM) variations.
Compute financial differentials in USD.
Detect "Daily Peaks" (anomalies in event volume).
Format the data into a responsive HTML Report


📧 6. Automated Executive Reporting
Sends a highly visual HTML email to stakeholders containing:
KPI Cards: Total Monthly Spend (USD).
Trend Tables: Weekly volume breakdown (01-08, 08-15, etc.).
Visual Alerts: 🔴 Red/Green indicators for positive/negative trends.
Rate Cards: Summary of contractual costs applied.

🧬 Workflow Architecture

<img width="1212" height="629" alt="Captura de pantalla 2026-01-06 100608" src="https://github.com/user-attachments/assets/cc986acd-9117-4202-8f4d-003ebf213f70" />

