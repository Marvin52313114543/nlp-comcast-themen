## Verwendung Code/Projekt
1. Repository klonen und in den Projektordner wechseln:
```bash
git clone https://github.com/Marvin52313114543/nlp-comcast-themen.git
cd nlp-comcast-themen
```

2. Kaggle Datensatz herunterladen und hier ablegen:
data/comcast_consumeraffairs_complaints.csv

3. Virtuelle Umgebung erstellen und aktivieren:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

4. Pakete installieren
```bash
pip install -r requirements.txt
```

5. NLTK-Ressourcen einmalig herunterladen:
```bash
python -c "import nltk; nltk.download('punkt'); nltk.download('punkt_tab'); nltk.download('stopwords'); nltk.download('wordnet'); nltk.download('omw-1.4')"
```

6. Projekt starten
```bash
jupyter lab
```

## Data
CSV wird nicht ins Repository hochgeladen. Bitte Datensatz von Kaggle herunterladen und unter `data/comcast_consumeraffairs_complaints.csv` ablegen.

Link zum Kaggle Datensatz: https://www.kaggle.com/datasets/archaeocharlie/comcastcomplaints?resource=download&select=comcast_consumeraffairs_complaints.csv


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

