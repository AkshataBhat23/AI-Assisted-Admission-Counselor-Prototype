# 🎓 AI-Assisted Admission Counselor Prototype

A Python-based command-line tool that acts as an AI-driven college admissions counselor. This system takes a student's academic profile (interests, strengths, weaknesses, and preferences) and generates:

- A personalized SWOT analysis (with LLM-based Opportunities and Threats)
- Matched university programs (scraped or mock-based)
- Tailored academic advice using OpenRouter AI models

---

## ✨ Features

- ✅ **Student Input** via command-line
- ✅ **SWOT Analysis Engine** powered by OpenRouter (`mistral-7b-instruct`)
- ✅ **Real-world Program Matching** via web scraping or mock dataset
- ✅ **LLM-generated Advice** customized for the student profile
- ✅ **Modular, well-commented code** for easy understanding and extension

---

## 🧠 How It Works

### ➤ 1. Input Module

Takes student input such as:
- Academic interests (e.g. `AI`, `Robotics`)
- Strengths (e.g. `math`, `leadership`)
- Weaknesses (e.g. `low confidence`)
- Preferences (e.g. location: `Mumbai`)

### ➤ 2. SWOT Analysis

- `Strengths` and `Weaknesses` are input manually
- `Opportunities` and `Threats` are generated dynamically using **OpenRouter AI**

### ➤ 3. Program Matching

- Scrapes data from real university websites (e.g., SCOE, VJTI, ACE)
- Optionally uses mock data if scraping fails
- Filters results based on interests and preferences

### ➤ 4. LLM-Powered Advice

- Uses OpenRouter's `mistral-7b-instruct` to:
  - Offer personalized application advice
  - Motivate the student
  - Recommend strengths to highlight in SOP

---

## 🚀 Quick Start

### 🔧 Requirements

- Python 3.7+
- `requests`, `beautifulsoup4`, `python-dotenv`

```bash
pip install requests beautifulsoup4 python-dotenv
