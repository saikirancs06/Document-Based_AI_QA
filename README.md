# 📄 Document-Based AI Question Answering System

An AI-powered web application that analyzes PDF resumes, compares candidate skills against job descriptions, and answers questions using Google's Gemini Generative AI.

🔗 **Live Demo:** [Try the application](https://document-basedaiapp-ofhu8gab3eb9nqnkjcbewy.streamlit.app/)

## 🚀 Project Overview

The Document-Based AI Question Answering System helps users extract information from resumes, identify matching and missing skills, and ask questions about candidate qualifications.

The application combines document processing, keyword-based skill matching, and Generative AI to provide structured answers based on the uploaded resume and job description.

## ✨ Features

- **PDF Text Extraction:** Extracts readable text from uploaded resume PDFs using PyMuPDF.
- **Skill Matching:** Compares skills mentioned in a job description against the resume.
- **Missing Skill Identification:** Highlights skills from the application's supported skill list that were not found in the resume.
- **Match Score:** Calculates a keyword-based skill match percentage.
- **AI-Powered Question Answering:** Uses Google's Gemini API to answer questions about resume content and job requirements.
- **Interactive Web Interface:** Provides a simple interface built with Streamlit.
- **Cloud Deployment:** Published using Streamlit Community Cloud.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Application development |
| Streamlit | Interactive web interface |
| Google Gemini API | Generative AI question answering |
| Google GenAI SDK | Gemini API integration |
| PyMuPDF | PDF text extraction |
| Pandas | Data manipulation dependency, if used |
| Git and GitHub | Version control and source code hosting |
| Streamlit Community Cloud | Application deployment |

## ⚙️ How It Works

1. Upload a resume in PDF format.
2. Extract the text from the uploaded document.
3. Paste the target job description.
4. Compare resume keywords against supported job skills.
5. Review matched skills, missing skills, and the keyword match score.
6. Enter a question about the resume or job description.
7. Receive an AI-generated answer from Gemini.

## 📂 Project Structure

```text
Document_AI_QA/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── .streamlit/
    └── secrets.toml   # Local secret file; never commit
```

## 💻 Local Installation and Setup

### Prerequisites

- Python 3.10 or a compatible version
- A Google Gemini API key
- Git (optional, for cloning the repository)

### 1. Clone the Repository

```bash
git clone https://github.com/saikirancs06/Document-Based_AI_QA
cd document-ai-qa
```

Replace `https://github.com/saikirancs06/Document-Based_AI_QA` with the HTTPS URL of your GitHub repository.

Alternatively, download the repository as a ZIP file and extract it.

### 2. Create and Activate a Virtual Environment

```bash
python -m venv .venv
```

**Windows:**

```bash
.venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the Gemini API Key

Create a file named `.streamlit/secrets.toml` and add:

```toml
GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"
```

Replace the placeholder with your actual API key from [Google AI Studio](https://aistudio.google.com/apikey).

Never upload this file or expose your API key publicly.

### 5. Run the Application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal, usually `http://localhost:8501`.

## ☁️ Deployment on Streamlit Community Cloud

1. Push the application code to a GitHub repository.
2. Open [Streamlit Community Cloud](https://share.streamlit.io/).
3. Connect your GitHub account.
4. Create an app and select your repository, branch, and `app.py`.
5. Open the app's settings and configure `GEMINI_API_KEY` in the Secrets section using valid TOML syntax.
6. Deploy the application and open the generated public URL.

## 🔐 Security Considerations

- Store API keys in Streamlit Secrets or environment variables.
- Exclude `.streamlit/secrets.toml`, `.env`, and private documents from Git commits.
- Use sample or anonymized resumes for demonstrations.
- Review AI-generated answers before relying on them.
- Avoid using the application as the sole basis for recruitment decisions.

## ⚠️ Limitations

- Skill matching is based on keywords and may not understand synonyms or context.
- The match score is not a validated measure of candidate suitability.
- Scanned PDFs may require OCR before text can be extracted.
- AI-generated answers may be incomplete or inaccurate.
- Gemini API availability and usage limits depend on the account and current service terms.

## 🎯 Skills Demonstrated

Python Programming · Generative AI · API Integration · Prompt Engineering · PDF Processing · Text Analysis · Streamlit · GitHub · Cloud Deployment

## 🔮 Future Enhancements

- Add OCR support for scanned resumes.
- Expand skill matching with semantic similarity.
- Support multiple document formats.
- Add downloadable candidate analysis reports.
- Improve error handling and document validation.
- Add automated tests and application monitoring.

## 👨‍💻 Author

**C S Sai Kiran**

Aspiring Data Analyst / Data Science Professional

---

*This project was developed for learning, portfolio demonstration, and experimentation with document-based Generative AI.*
