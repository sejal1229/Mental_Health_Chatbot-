#  Mental Health Chatbot – 🤍

A calm and comforting AI therapy chatbot that talks like your best friend  
Built with LLaMA2 (via Ollama), FAISS vector search, and an empathetic tone — it listens when you need it most.

---

##  Features

-  Calm, supportive replies using LLaMA (TinyLLaMA via Ollama)
-  FAISS-based semantic answer search from curated mental health dataset
-  Human-style rewrites with warm emojis (like 🤍, 😊, 🌿)
-  HTML-based chat UI (Bootstrap 5)
-  Flask backend with POST endpoint for AI replies
-  KS branded favicon and styling

---

##  Folder Structure

```
project/
├── app.py                     # Flask server
├── index.html                 # Frontend UI
├── chatbot_llama.py           # FAISS + LLaMA integration
├── generate_faiss.py          # Builds FAISS index
├── mentalhealth.csv           # Dataset (Questions + Answers)
├── answers.pkl                # Pickled answers list
├── faiss_index.index          # FAISS index file
├── static/
│   └── favicon.ico           
└── site.webmanifest           # (optional PWA support)
```

---

##  Setup Instructions

1.  Make sure you have Ollama + TinyLLaMA installed:
```bash
ollama pull tinyllama
```

2.  Install Python dependencies:
```bash
pip install flask flask-cors faiss-cpu sentence-transformers
```

3.  Generate FAISS index:
```bash
python generate_faiss.py
```

4.  Run the app:
```bash
python app.py
```

Then open your browser at http://127.0.0.1:5000

---

##  How It Works

- You ask a question → frontend sends to Flask via POST
- Flask uses SentenceTransformer to embed your query
- FAISS finds the closest matching answer
- LLaMA rewrites it to sound like a warm, caring friend using natural emojis
- The response is shown in a friendly bubble chat UI 🫶

---

##  Customization

Want your own logo?

- Replace favicon.ico in /static/  
- Or update <link rel="icon"> in index.html to point to your image

---

##  Made With Love by Sejal

This project is more than just code — it's care ❤️  
If you or someone you know needs help, this chatbot is a small digital shoulder to lean on.

> “You got this. One deep breath at a time.” 🤍

---

## 📃 License

MIT License — feel free to use, modify, share.
