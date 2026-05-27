# ATS Resume Scorer

A web app that scores how well a resume matches a job description and returns actionable feedback. Built with FastAPI + Streamlit, using spaCy and Sentence Transformers for NLP and the Groq API for LLM-generated suggestions.


# What it does
1. Upload a resume (PDF / DOC / DOCX) and paste a job description.
2. The backend parses the resume, extracts skills and experience, and compares them to the JD using semantic similarity.
3. You get an ATS score, a breakdown by category (formatting, keywords, content, skill validation, ATS compatibility), and LLM-written suggestions for what to improve.
4. Past analyses are saved to your account so you can revisit them.

## Tech Stack

**Frontend:** Streamlit
**Backend:** FastAPI
**NLP:** spaCy, Sentence Transformers
**LLM:** Groq API (Llama 3)
**Database & Authentication:** Supabase

# Run Backend 
uvicorn backend.main:app --reload

# Run Frontend 
streamlit run frontend/streamlit_app.py



