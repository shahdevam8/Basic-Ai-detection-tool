🛡️ AegisText — Independent AI Text Detection Tool
AegisText is an offline, explainable AI-generated text detection tool designed to analyze any given text and estimate how likely it is to be AI-generated vs human-written, expressed as a percentage probability.

The project is fully independent, does not rely on external APIs, and works across most modern AI text generators (ChatGPT, Gemini, Claude, LLaMA, paraphrasers, etc.).

🚀 Key Highlights
🔍 Detects AI-generated vs Human-written text

📊 Outputs AI probability percentage

🧠 Uses multi-signal ensemble detection

🔐 Fully offline & private

🧩 Explainable results (feature-level breakdown)

🎨 Professional UI (Streamlit)

⚙️ Modular, extensible architecture

📁 Project Folder Structure
ai-text-detector/
├── app.py                 # Streamlit UI entry point
├── ensemble.py            # Aggregates detection scores
├── detector.py            # Core AI vs Human logic
├── features.py            # Linguistic & statistical features
├── requirements.txt       # Project dependencies
├── README.md              # Project documentation
└── venv/                  # Virtual environment (optional)
📦 Requirements
Python Version
Python 3.10.x (recommended)

⚠️ Avoid Microsoft Store Python for ML projects due to binary incompatibility issues.

requirements.txt
nltk==3.8.1
numpy==1.26.4
torch==2.1.2
transformers==4.41.2
scikit-learn==1.3.2
spacy==3.7.2
tqdm==4.66.1
streamlit==1.35.0
One-Time Setup (Required)
python -m spacy download en*core*web_sm
python - <<EOF
import nltk
nltk.download("punkt")
nltk.download("punkt_tab")
EOF
🧠 How AegisText Works
AegisText uses an ensemble-based detection approach instead of relying on a single unreliable signal.

Detection Signals Used
Signal	What It Measures
Lexical Diversity	Vocabulary richness vs repetition
Entropy	Predictability of word distribution
Repetition Score	Repeated phrasing common in AI text
Sentence Variance	Uniform vs natural sentence length
Stylometric Patterns	Human vs machine writing rhythm
Semantic Consistency	Overly coherent AI transitions
Each signal contributes to a weighted final score, producing:

AI Generated Probability (%)

Human Written Probability (%)

📊 Example Output
AI Generated Probability: 71.8%
Human Written Probability: 28.2%

Verdict: Likely AI Generated
For ambiguous or mixed content:

AI Generated Probability: 45.3%
Verdict: Mixed / Uncertain
🖥️ How to Use
1️⃣ Clone or Download the Project
git clone https://github.com/yourusername/ai-text-detector.git
cd ai-text-detector
2️⃣ Create Virtual Environment (Recommended)
python -m venv venv
venv\Scripts\activate
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Run the Application
streamlit run app.py
The UI will open automatically in your browser.

🎨 User Interface Overview
📝 Text input area

🔍 Analyze button

📊 AI vs Human probability

🧩 Feature-level breakdown

⚠️ Warnings for short or uncertain text

🌙 Clean, professional dark theme

🎯 Capability & Accuracy
What It Does Well
Detects pure AI-generated content

Flags paraphrased AI text

Handles mixed human + AI writing

Works across multiple AI models

Offline & privacy-first

Important Limitations (Honest Disclosure)
❌ Cannot guarantee 100% accuracy

❌ Heavily edited AI text may evade detection

❌ Very short text reduces reliability

⚠️ Any tool claiming “100% AI detection” is misleading.

🔐 Privacy & Independence
No APIs

No cloud calls

No data logging

No tracking

Everything runs locally

🧩 Potential Upgrades & Roadmap
This project is designed to be future-proof and extensible.

🔮 Possible Enhancements
📄 PDF / DOCX upload support

🧠 Perplexity-based LLM scoring

🎯 Sentence-level AI highlighting

📊 Visual confidence graphs

🌐 REST API / SaaS deployment

🧩 Chrome Extension

🖥️ Desktop EXE (Windows / macOS)

📚 Academic integrity mode

🧪 Benchmark evaluation framework

🏆 Use Cases
Academic integrity checks

Content moderation

Journalism verification

SEO content auditing

Resume / portfolio project

Startup MVP

Research experiments
