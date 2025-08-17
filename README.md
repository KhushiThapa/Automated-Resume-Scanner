# Automated-Resume-Scanner
🤖 Smart ATS – An AI-powered resume screening system using Google Gemini &amp; Streamlit that extracts, analyzes, and matches resumes with job descriptions, giving JD match %, keywords &amp; summary.
# 📄 Smart ATS – Automated Resume Screening System  

## 📝 Overview  
The **Smart ATS** is an **AI-powered Automated Resume Screening System** that helps candidates and recruiters evaluate resumes against job descriptions.  
It uses **Google Gemini API**, **Streamlit**, and **NLP techniques** to:  
- 📄 Parse resumes from PDFs  
- 🎯 Match skills and keywords with job descriptions  
- 🤖 Generate ATS-friendly feedback including JD match %, missing keywords, and profile summary  

This project is designed to **streamline hiring** and **help job seekers optimize their resumes** to pass ATS filters.  

---

## 🚀 Features  
- 📑 **Resume Parsing** – Extracts text from uploaded PDF resumes  
- 🤖 **AI-Powered Analysis** – Uses Google Gemini (`gemini-pro`) for deep evaluation  
- 🎯 **JD Match %** – Calculates how well a resume matches the given job description  
- 🔑 **Keyword Suggestions** – Identifies missing keywords/skills  
- 📝 **Profile Summary** – Generates a professional ATS-friendly summary  
- 🖥️ **Interactive UI** – Built with Streamlit for easy use  

---

## 🏗️ Project Structure  

📂 Smart-ATS
┣ 📜 app.py # Main Streamlit app
┣ 📜 requirements.txt # Python dependencies
┣ 📜 .env.example # Environment variable template
┣ 📜 README.md # Project documentation
┣ 📂 assets/ # Screenshots, demo images (optional)
┗ 📂 data/ # Sample resumes/JDs (optional)

markdown
Copy
Edit

---

## ⚙️ Architecture  

1. **Input Layer**  
   - 📄 Resume Upload (PDF)  
   - 📝 Job Description Text  

2. **Processing Layer**  
   - 🔍 Resume text extraction (PyPDF2)  
   - 🧾 Prompt creation with JD + resume  
   - 🤖 AI analysis using Google Gemini (`gemini-pro`)  

3. **Output Layer**  
   - 🎯 JD Match %  
   - 🔑 Missing Keywords  
   - 📝 Profile Summary  

---

## 🛠️ Tech Stack  

- **Frontend / UI**: 🎨 Streamlit  
- **Backend**: 🐍 Python  
- **AI Model**: 🤖 Google Gemini (`gemini-pro`)  
- **Libraries**:  
  - 📄 PyPDF2 – PDF parsing  
  - 🔐 python-dotenv – Environment variables  
  - ⚙️ json, os – Utilities  
- **Deployment**: ☁️ Streamlit Cloud / Heroku / Docker  

---
## 📥 Installation & Setup  

### 1️⃣ **Clone Repository**  
```bash
git clone https://github.com/your-username/Smart-ATS.git
cd Smart-ATS
2️⃣ Create Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)
3️⃣ Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4️⃣ Set Environment Variables
Create a .env file in the root folder and add your Google API Key:

env
Copy
Edit
GOOGLE_API_KEY=your_api_key_here
5️⃣ Run the Application
bash
Copy
Edit
streamlit run app.py
