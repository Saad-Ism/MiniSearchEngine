# Mini Search Engine

A simple sentence-level search engine built from scratch using:

## Features
- Sentence-level chunking for fine-grained search
- `.docx` support (ideal for downloaded articles or notes)
- Custom preprocessing pipeline:
  - Tokenization
  - Stopword removal
  - Stemming (PorterStemmer)
- TF-IDF vectorization
- Cosine similarity scoring for best match retrieval
- Easily extensible for multi-sentence results, ranking, or summaries

MiniSearchEngine/
├── input.docx # Your input file (e.g., Wikipedia page)
├── main.py # Entry point
├── preprocessing.py # Tokenization, stopwords, stemming
├── docx_reader.py # .docx loader + sentence chunking
├── search_engine.py # TF-IDF + cosine similarity
├── requirements.txt # Dependencies
├── README.md # You're reading this!
└── nltk_data/ # (Optional) Local NLTK data folder

# How to Run
- Add your input file as input.docx
- Make sure you have the correct filepath to NLTK's PUNKT and Stopwords. You can either download in code (as follows), or give access to a local file
- nltk_data is excluded from version control to keep repo light.
- If you clone this repo, run the following to set up:
import nltk
nltk.download('punkt')
nltk.download('stopwords')

# Example Query
Enter a search query: gas giants
Top result: "Jupiter and Saturn are the largest gas giants in the solar system."

Built by Saad Ismail
Project based on real-world NLP course implementation using Python and NLTK.
