# MentorMatch – AI-Powered Mentorship Recommendation Platform

MentorMatch is a Flask web app that recommends mentors using sentence embeddings and cosine similarity.

## 🚀 Features
- Embedding-based search with `sentence-transformers` (`all-MiniLM-L6-v2`)
- `/find_mentor` JSON API + simple web UI (`templates/index.html`)
- Works with scraped mentors; optionally merges LinkedIn data if available

## 📂 Project Structure
- `app.py` – Flask app (loads data, serves UI & API)
- `encoding_mentors.py` – generates embeddings into `mentor_scraped_data.csv`
- `mentor_scraped_data.csv` – sample mentors (bios, skills, name, embedding)
- `DataLab_final_version.ipynb` – exploration/development notebook
- `templates/index.html` – minimal UI
- `requirements.txt` – dependencies

## ⚙️ Setup
```bash
pip install -r requirements.txt
