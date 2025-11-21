# Mental Health Chatbot – 🤍

An empathetic, human-touch AI chatbot for mental health support — built using TinyLLaMA, FAISS, and a beautifully designed HTML interface.

This repository contains 3 versions of the chatbot — all with the same backend, but with different levels of frontend user experience.

---

## Project Structure Overview

```

Mental\_health\_chatbot/
├── Mental\_health\_basic\_gui/              # Basic HTML interface version
│   ├── app.py
│   ├── chatbot\_llama.py
│   ├── generate\_faiss.py
│   ├── faiss\_index.index
│   ├── answers.pkl
│   ├── index.html
│   └── mentalhealth.csv

├── mental\_health\_simple\_gui/             # Improved layout (cleaner styling)
│   ├── (same structure as above)

├── mental\_health\_advanced\_ui/            # Final well-polished version with human-like responses
│   ├── app.py
│   ├── chatbot\_llama.py
│   ├── generate\_faiss.py
│   ├── index.html
│   ├── mentalhealth.csv
│   ├── answers.pkl
│   ├── faiss\_index.index
│   ├── site.webmanifest
│   └── static/
│       └── favicon.ico

````

Each folder contains a complete functional app with:

-  FAISS + sentence-transformers for semantic Q&A
-  LLaMA (via Ollama) to rewrite answers like a warm best friend
-  HTML front-end with different levels of styling

---

## Technologies Used

- FAISS for semantic similarity search  
- SentenceTransformers (MiniLM-L6-v2)  
- Ollama running TinyLLaMA locally  
- Flask API backend  
- HTML, CSS (Bootstrap 5), emojis and avatars for UI polish  

---

## Getting Started

1. Clone this repository:

```bash
git clone https://github.com/sejal1229/Mental_health_chatbot.git
cd Mental_health_chatbot/mental_health_advanced_ui
````

2. Install required packages:

```bash
pip install flask flask-cors faiss-cpu sentence-transformers
```

3. Pull TinyLLaMA via Ollama:

```bash
ollama pull tinyllama
```

4. Generate FAISS index (only once):

```bash
python generate_faiss.py
```

5. Start Flask backend:

```bash
python app.py
```

6. Open your browser at:
   [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## Chatbot with Human Touch

* Rewrites robotic responses into soothing, caring replies
* Includes friendly tone, calm affirmations, and gentle emojis like 🤍, 🌿, 😊
* UI designed to feel like a safe, cozy chatroom 

---

##  UI Versions

| Folder                       | Description                            |
| ---------------------------- | -------------------------------------- |
| Mental\_health\_basic\_gui   | Basic starting point UI (plain layout) |
| mental\_health\_simple\_gui  | Improved visual layout                 |
| mental\_health\_advanced\_ui | Final polished design + emojis + logo  |

Choose the one that suits your use case or audience.

---

##  Developed By

Made with ❤️ and care by [Sejal Singh](https://github.com/sejal1229)

> "Sometimes, just having someone who listens makes all the difference." 🤍

---

## 📄 License

MIT License — free to use, modify, and share for education or wellness projects.
