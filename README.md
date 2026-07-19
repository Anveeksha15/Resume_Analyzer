## 📄 Resume Analyzer & Enhancer 

A simple yet powerful Streamlit-based web app that allows users to upload their resume and a job/internship description to receive an in-depth analysis including ATS score, SWOT analysis, missing keywords, and personalized improvement suggestions.

---

### 🚀 Features

* Upload your **PDF resume**
* Paste the **job/internship description**
* Get:

  * ✅ **ATS Score** (with improvement suggestions)
  * ✅ **SWOT Analysis** (Strengths, Weaknesses, Opportunities, Threats)
  * ✅ **Top 5 Missing Keywords**
  * ✅ **Content & Formatting Tips**
  * ✅ **Selection Probability Estimate**

---

### 🛠 Tech Stack

* **Frontend**: [Streamlit](https://streamlit.io/)
* **Backend**:

  * `PyMuPDF` or `pdfplumber` for PDF text extraction
  * `OpenAI GPT-4` for resume analysis and feedback
* **Environment**: Python 3.8+, dotenv for API key management

---

### 📦 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Anveeksha15/Resume_Analyzer.git
   cd resume-analyzer
   ```

2. **Create a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up your `.env` file**
   Create a `.env` file in the root directory and add:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   ```

---

### 📂 File Structure

```
resume-analyzer/
├── backend/
│   ├── extractor.py        # Extracts text from uploaded PDF
│   └── analyzer.py         # Sends resume + job desc to GPT and returns analysis
├── .env                    # API key (not included in repo)
├── app.py                  # Streamlit frontend
├── requirements.txt        # Python dependencies
└── README.md               # You're reading it!
```

---

### ▶️ Run the App

```bash
streamlit run app.py
```

---

### 📌 To-Do (Ideas for Improvement)

* Add support for `.docx` resumes
* Export analysis report as PDF
* Add keyword cloud visualization
* Integrate with LinkedIn job scraping
* Add AI resume generator/fixer

