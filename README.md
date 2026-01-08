# 🛡️ AegisText --- Independent AI Text Detection Tool

AegisText is an **offline, explainable AI-generated text detection
tool** designed to analyze any given text and estimate **how likely it
is to be AI-generated vs human-written**, expressed as a **percentage
probability**.

The project is fully **independent**, does **not rely on external
APIs**, and works across **most modern AI text generators** (ChatGPT,
Gemini, Claude, LLaMA, paraphrasers, etc.).

------------------------------------------------------------------------

## 🚀 Key Highlights

-   🔍 Detects **AI-generated vs Human-written text**
-   📊 Outputs **AI probability percentage**
-   🧠 Uses **multi-signal ensemble detection**
-   🔐 Fully **offline & private**
-   🧩 Explainable results (feature-level breakdown)
-   🎨 Professional UI (Streamlit)
-   ⚙️ Modular, extensible architecture

------------------------------------------------------------------------

## 📁 Project Folder Structure

    ai-text-detector/
    ├── app.py
    ├── ensemble.py
    ├── detector.py
    ├── features.py
    ├── requirements.txt
    ├── README.md
    └── venv/

------------------------------------------------------------------------

## 📦 Requirements

### Python Version

-   **Python 3.10.x (recommended)**

### requirements.txt

    nltk==3.8.1
    numpy==1.26.4
    torch==2.1.2
    transformers==4.41.2
    scikit-learn==1.3.2
    spacy==3.7.2
    tqdm==4.66.1
    streamlit==1.35.0

------------------------------------------------------------------------

## 🧠 How It Works

AegisText uses an **ensemble-based detection approach** combining
linguistic, statistical, and semantic signals to estimate AI
probability.

Signals include: - Lexical diversity - Entropy - Repetition patterns -
Sentence variance - Stylometry - Semantic predictability

Each signal contributes to a weighted final score.

------------------------------------------------------------------------

## 🖥️ How to Use

``` bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

------------------------------------------------------------------------

## 🎯 Capability & Accuracy

-   Effective for pure AI-generated content
-   Detects paraphrased and mixed content
-   Offline and privacy-first

⚠️ No AI detector can guarantee 100% accuracy.

------------------------------------------------------------------------

## 🔮 Future Enhancements

-   Sentence-level highlighting
-   PDF/DOCX upload
-   REST API
-   Chrome extension
-   Desktop EXE
-   Benchmark framework
