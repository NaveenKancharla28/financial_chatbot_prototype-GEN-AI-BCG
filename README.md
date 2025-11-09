markdown# Financial Analysis Chatbot Prototype  
**BCG GEN-AI Certification Project**  
*Submitted by: Naveen Chaitanya Kancharla*

---

## Project Overview
A **rule-based financial chatbot** that answers **predefined queries** using real 10-K data from **Microsoft, Tesla, and Apple** (FY2022–FY2025).  
Built using **Python + Pandas** for data processing and **command-line interaction**.

---

## Predefined Queries (Exact or Keyword Match)

| Query | Example Response |
|------|------------------|
| `What is Microsoft's total revenue?` | Microsoft's total revenue in FY2025 is $268,877 million. |
| `How has Tesla's net income changed?` | Tesla's net income decreased from $14,997M to $7,093M (-52.7%) in FY2024. |
| `What is Apple's cash flow from operating activities?` | Apple generated $118,254 million in cash flow from operating activities in FY2024. |

> Case-insensitive. Partial keyword match supported.

---

## How It Works

1. **Data Source**: `data_summary.xlsx` (extracted from SEC EDGAR 10-K filings)
2. **Logic**: `if-elif` with keyword matching and YoY calculations
3. **Interaction**: Terminal-based using `input()`
4. **No external APIs or NLP** — lightweight and reliable

---

## Setup & Run

```bash
# 1. Clone repo
git clone https://github.com/NaveenKancharla28/financial_chatbot_prototype-GEN-AI-BCG.git
cd financial_chatbot_prototype-GEN-AI-BCG

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run chatbot
python chatbot.py
```
Sample Interaction
textFinancial Analysis Chatbot (Type 'quit' to exit)

You: What is Microsoft's total revenue?
Bot: Microsoft's total revenue in FY2025 is $268,877 million.

You: How has Tesla's net income changed?
Bot: Tesla's net income decreased from $14,997M to $7,093M (-52.7%) in FY2024.

You: quit
Bot: Goodbye!

Limitations

Only supports 3 predefined query types
No natural language understanding (NLU)
Command-line only (no web UI)
Static data (not real-time)




Certification Compliance



































RequirementMet?EvidenceData from real 10-K filingsYesdata_summary.xlsx with source links in commentsFunctional chatbotYeschatbot.py with tested responsesClear documentationYesThis README.mdVersion controlYesGitHub repo with commit historyReproducibleYesrequirements.txt + setup steps

Author
Naveen Chaitanya Kancharla
GitHub | LinkedIn
BCG Generative AI Certification — Final Project Submission

text---

## 2. `.gitignore`

```gitignore
# Ignore large or generated files
*.zip
__pycache__/
*.pyc
.DS_Store

3. LICENSE (MIT – Standard for Certifications)
txtMIT License

Copyright (c) 2025 Naveen Chaitanya Kancharla

Permission is hereby granted, free of charge, to any person obtaining a copy...
(Copy full MIT from here)

4. requirements.txt
txtpandas
openpyxl
