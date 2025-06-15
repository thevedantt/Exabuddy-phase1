📚 AI PDF Summarizer (with Manual + Gemini AI Summary)
This project provides an interactive, accurate, and concise summarization of any academic or research PDF. It generates both a manual summary (rule-based) and an AI-generated summary (using Google's Gemini 2.0 Flash model). It also extracts keywords, key phrases, and basic text statistics.

🚀 Features
✅ Extract text from uploaded PDF files.

🧠 Manual Summary: Extractive, based on meaningful sentences.

🤖 AI Summary: Gemini-generated abstract based on context and keywords.

🔍 Keyword extraction: Most frequent informative terms.

📌 Phrase extraction: Key noun chunks (multi-word concepts).

📊 Statistics: Total word count for the document.

💡 Fully runs in Google Colab (no local setup required).

🔧 Tech Stack
Python 3

Google Colab

Google Generative AI (Gemini 2.0 Flash)

NLTK

spaCy

PyPDF2

📂 Use Cases
Use Case	Description
🎓 Academic Summaries	Generate concise summaries of research papers, theses, or e-books.
🧪 Research Assistance	Extract key concepts from large scientific texts.
📚 Study Notes	Turn class notes into short revision points.
📈 Business Reports	Summarize reports and proposals for quick decision making.
🤖 AI Text Preprocessing	Prepare datasets for NLP models using clean, reduced, and keyword-rich text.

🛠️ Setup & Installation
💻 No local installation required – just use Google Colab.

1. Open the Colab Notebook
Go to Google Colab and paste your code.

Or use: File → Upload Notebook if you already exported it.

2. Install Dependencies (Automatically handled in Colab)
These are included:

bash
Copy
Edit
pip install PyPDF2 google-generativeai nltk spacy
python -m spacy download en_core_web_sm
3. Upload a PDF
The code will prompt:

css
Copy
Edit
📁 Upload a PDF file:
Choose your file (e.g., ML.pdf), and it will begin processing.

🧠 How It Works
➤ Step-by-step Pipeline
PDF Upload
→ File uploaded via Google Colab

Text Extraction
→ PyPDF2 reads and extracts all text from pages.

Cleaning & Preprocessing
→ Punctuation, extra whitespaces removed; tokenization applied.

Manual Summary
→ The first few meaningful sentences are selected as a rough overview.

Keyword & Phrase Extraction
→ Uses nltk and spaCy to extract most frequent terms and noun phrases.

AI Summary (Gemini)
→ Gemini Flash model generates a 100-word abstract using keywords.

Output Displayed
→ You get:

Manual summary

AI summary

Keywords

Key phrases

Word count

📌 Sample Output
yaml
Copy
Edit
📄 Processing: ml_research.pdf
✅ Extracted from 12 pages

📚 MANUAL SUMMARY:
Machine learning enables systems to learn and improve...

🤖 AI-GENERATED SUMMARY:
This paper discusses supervised learning approaches...

🔑 KEYWORDS:
learning, algorithm, model, accuracy, dataset...

🧩 KEY PHRASES:
machine learning algorithm, test dataset, training model...

📊 STATISTICS:
Word Count: 3,268
🔐 API Key Note
This project uses the Gemini 2.0 Flash model via:

python
Copy
Edit
genai.configure(api_key="YOUR_API_KEY")
Replace "YOUR_API_KEY" with your Google Generative AI API key.
🔑 Get an API Key here

✅ Best Practices
Use academic or structured PDF files (text-based, not scanned images).

Summaries work best with content that’s technical or domain-specific.

Avoid uploading encrypted or non-readable PDFs.

📌 Future Enhancements
Save summaries and keywords to Google Drive or Sheets.

Convert summaries to bullet points or mind maps.

Support OCR for image-based PDFs.

Language detection and multilingual summaries.

🧑‍💻 Author
Vedant Talekar

For questions or improvements, feel free to message or fork!

📜 License
This project is for educational and personal use.
Model usage depends on Google AI Terms & Policies.

