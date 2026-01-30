# NLP Topic Extraction – Comcast Complaints

Analyse von Beschwerdetexten mit NLP (BoW/TF-IDF, LSA, LDA).
Link zum GitHub-Repository: https://github.com/Marvin52313114543/nlp-comcast-themen

## Data
CSV wird nicht ins Repository hochgeladen. Bitte Datensatz von Kaggle herunterladen und unter `data/comcast_consumeraffairs_complaints.csv` ablegen.

Link zum Kaggle Datensatz: https://www.kaggle.com/datasets/archaeocharlie/comcastcomplaints?resource=download&select=comcast_consumeraffairs_complaints.csv

## Setup (macOS)
```bash
# Virtuelle Umgebung erstellen
python3 -m venv .venv
# Virtuelle Umgebung aktivieren
source .venv/bin/activate
# Pakete installieren
pip install -r requirements.txt
# NLTK Ressourcen einmalig herunterladen
python -c "import nltk; nltk.download('punkt'); nltk.download('punkt_tab'); nltk.download('stopwords'); nltk.download('wordnet'); nltk.download('omw-1.4')"

```

## Import und Tokenisierungstest
```bash
#Importtest
python -c "import pandas, sklearn, nltk, contractions; print('OK')"
#Tokenisierungstest
python -c "import nltk; from nltk.tokenize import word_tokenize; print(word_tokenize('This is a test.'))"

```

## Weitere Befehle die im Projekt verwendet wurden
```bash
# Projektordner erstellen und in diesen wechseln
mkdir nlp-comcast-themen
cd nlp-comcast-themen

# requirements.txt erstellen
pip freeze > requirements.txt

# Pip installieren und aktualisieren falls nicht installiert oder aktuell
python -m pip install --upgrade pip

# Falls Conda aktiviert ist muss es deaktiviert werden
conda deactivate

# öffnen von Jupyter Lab
jupyter lab
```

