# 🧠 PiP Install BigBoss (Memory Search System)

A lightweight local AI memory pipeline that turns folders of code, text, PDFs, and images into searchable knowledge.

It extracts content, splits files into chunks, creates smart summaries using embeddings, builds vector memory, and lets you search everything with one sentence.

---

# ✨ Core Features

| Feature              | Description                            |
| -------------------- | -------------------------------------- |
| 📂 Folder Ingestion  | Scan any folder recursively            |
| 🧾 Text Support      | TXT, MD, CSV, JSON, logs               |
| 💻 Code Support      | Python, JS, HTML, CSS, C++, etc        |
| 📄 PDF Support       | Selectable PDF text extraction         |
| 🖼️ Image OCR        | Optional PNG/JPG text detection        |
| ✂️ Smart Chunking    | Split large files into semantic chunks |
| 🧠 Embedding Summary | Keep top ~10% important text           |
| 🔎 Semantic Search   | Find best chunk from one sentence      |
| ⚡ Local First        | Runs on your own machine               |
| 🧱 Modular Design    | Easy to replace components             |

---

# 🗂️ Project Structure

```txt
BigBoss/
├── bigboss.py
├── base.py
├── check.py
├── embedding.py
├── code2chunk.py
├── txt2chunk.py
├── pic2textV2.py
├── chunks2contents.py
├── requirements.txt
├── memory/
│   ├── code2text/
│   ├── text2chunk/
│   ├── pic2text/
│   ├── chunk2contents/
│   └── embeddings/
```

---

# 🔄 Workflow

```txt
Input Folder
   ↓
Detect File Types
   ↓
Extract Text / OCR / Code Read
   ↓
Chunk Files into Parts
   ↓
Embedding Summary (~10%)
   ↓
Build Vector Memory
   ↓
One Sentence Search
```

---

# ⚙️ Installation

```bash
pip install -r requirements.txt
```

Optional OCR for images:

```bash
Install Tesseract OCR
```

---

# 🚀 Usage

## Build Memory

```bash
python bigboss.py --folder "C:\YourFolder" --chunk-size 500 --embed
```

## Search Memory

```bash
python check.py --query "how does this project process pdf files?"
```

---

# 🧠 Example Search Output

| Rank | File             | Match Score |
| ---- | ---------------- | ----------- |
| 🥇 1 | pdf_processor.py | 0.92        |
| 🥈 2 | OCR_notes.txt    | 0.88        |
| 🥉 3 | chunk_reader.py  | 0.84        |

---

# 🎯 Why This Project?

✅ No cloud needed
✅ Search your own files semantically
✅ Useful for codebases, notes, research, archives
✅ Replace manual browsing with AI retrieval

---

# 🔮 Future Ideas

| Upgrade                | Benefit                   |
| ---------------------- | ------------------------- |
| ⚡ Realtime Watcher     | Auto-update embeddings    |
| 🌐 Streamlit UI        | Beautiful local interface |
| 🗣️ Chat Mode          | Ask your files questions  |
| 🧠 Better Embeddings   | Stronger search quality   |
| 📊 Visual Memory Graph | Understand relationships  |

---

# ❤️ Philosophy

Your folders are not chaos.
They are memory waiting to become searchable.

---

# 📜 License

Open-source

---
