# NLP Topic Extraction – Comcast Complaints

Analyse von Beschwerdetexten mit NLP (BoW/TF-IDF, LSA, LDA).

## Setup (macOS)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -c "import nltk; nltk.download('punkt'); nltk.download('punkt_tab'); nltk.download('stopwords'); nltk.download('wordnet'); nltk.download('omw-1.4')"

ls
