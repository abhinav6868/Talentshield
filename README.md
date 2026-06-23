# TalentShield – AI Resume Screening Platform

An AI-powered resume screening platform that automates candidate shortlisting using OpenAI embeddings and semantic similarity scoring. Built as a full-stack Django web application.

---

## What It Does

Traditional resume screening is slow and keyword-dependent. TalentShield uses LLM-powered semantic search to understand the *meaning* behind resumes and job descriptions — not just exact keyword matches — ranking candidates by actual fit.

---

## Features

- **AI Resume Parsing** — Automatically extracts skills, experience, and qualifications from PDF and DOCX resumes via OpenAI API
- **Semantic Similarity Scoring** — Matches resumes to job descriptions using OpenAI vector embeddings, ranking candidates by relevance
- **HR Manager Dashboard** — Upload job descriptions, view ranked candidate list, download screening reports
- **Candidate Dashboard** — Upload resume, view match results, track application status
- **Resume Builder** — Built-in resume builder with downloadable templates
- **Role-Based Access** — Separate login flows for HR managers and candidates
- **Full Authentication** — Signup, login, and session management

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Django |
| AI / NLP | OpenAI API, OpenAI Embeddings, Semantic Search |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |
| File Handling | PDF & DOCX parsing |

---

## Project Structure

```
Demo 2/
├── manage.py
├── requirements.txt
├── Demo/                  # Django project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── talentshield/          # Main application
    ├── models.py
    ├── views.py
    ├── urls.py
    ├── forms.py
    ├── simple_ats_analyzer.py
    ├── templates/
    │   ├── index.html
    │   ├── login.html
    │   ├── signup.html
    │   ├── hrmanager.html
    │   ├── candidate.html
    │   ├── upload.html
    │   ├── results.html
    │   ├── profile.html
    │   └── resumebuilder.html
    └── static/
```

---

## Getting Started

### Prerequisites
- Python 3.10+
- MySQL
- OpenAI API key

### Installation

```bash
# Clone the repo
git clone https://github.com/abhinav6868/Talentshield.git
cd Talentshield

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Environment Setup

Create a `.env` file in the root directory:

```
OPENAI_API_KEY=your_openai_api_key
DATABASE_NAME=your_db_name
DATABASE_USER=your_db_user
DATABASE_PASSWORD=your_db_password
```

### Run the App

```bash
python manage.py migrate
python manage.py runserver
```

Visit `http://localhost:8000`

---

## Key Highlight

> Reduced manual resume shortlisting effort by an estimated **60–70%** by replacing keyword matching with semantic AI scoring.

---

## Author

**Abhinav Samuel**  
[LinkedIn](https://linkedin.com/in/abhinav-samuel-aa9b00343) · [GitHub](https://github.com/abhinav6868)
