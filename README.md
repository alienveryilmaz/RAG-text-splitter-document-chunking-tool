# 🧩 Text Chunker — Smart Text Chunking for RAG

**Text Chunker** is a lightweight, browser-based tool that splits long texts into sentence-aware chunks with configurable overlap — perfect for **RAG pipelines**, **embeddings**, and **vector database ingestion**.  
Everything runs locally in your browser — no server, no setup, no dependencies.

---

## ✨ Features

- ✂️ **Sentence-Aware Chunking** — Splits text intelligently by sentence boundaries for cleaner, context-aware results.  
- 🔗 **Configurable Overlap** — Preserves context between chunks (default 12%).  
- 📊 **Detailed Stats** — Displays total word count, chunk count, and average chunk size.  
- 📋 **One-Click Copy** — Instantly copy any chunk to your clipboard.  
- 💻 **100% Client-Side** — Works fully offline; no backend required.  
- 🎨 **Modern UI** — Clean, responsive design built with pure HTML, CSS, and JavaScript.  

---

## 🧠 How It Works

1. **Sentence Splitting**  
   The text is scanned for sentence-ending punctuation (`.`, `!`, `?`, `।`, `。`) and split accordingly.  

2. **Balanced Chunking**  
   Sentences are grouped dynamically to balance word counts across chunks without exceeding the maximum limit.  

3. **Context Overlap**  
   Each chunk (except the first) includes a small portion (~12%) of the previous chunk’s tail sentences to maintain semantic continuity — ideal for **RAG**, **LLMs**, or **embedding generation**.

---

## ⚙️ Configuration

All settings can be adjusted from the app interface (⚙️ Configuration Settings) or directly via code.

| Setting | Default | Description |
|----------|----------|-------------|
| **Max Chunk Size (words)** | `400` | Maximum word count per chunk. |
| **Overlap Percentage** | `12` | Percentage of previous chunk words to overlap. |
| **Overlap Flexibility** | `1.5` | Allows up to 1.5× overlap range to include full sentences. |

---

## 🚀 Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>

2. Open the file textChunkerRagTool.html in your browser.
3. Paste your text, adjust settings if needed, and click “Chunk Text”.
4. Copy chunks easily using the 📋 Copy buttons.

📊 Interface Overview
-   📥 Input Section — Paste or write the text you want to chunk.
-   📈 Stats Panel — Displays total word count, chunk count, and average size.
-   📤 Chunked Output — Lists each chunk with overlap information and a copy button.
-   ⚙️ Settings Panel — Configure chunk size and overlap interactively.

🔒 Privacy
-   All processing occurs entirely in your browser.
-   No data is sent to external servers — safe for confidential or private text.

🧩 Tech Stack
- HTML5
- CSS3
- Vanilla JavaScript
No external dependencies or frameworks required. Works on all modern browsers.

🗺️ Roadmap Ideas
-   🧾 Export chunks as JSON / TXT
-   🧠 Add token-based chunking (e.g., using tiktoken)
-   🌍 Multilingual sentence detection
-   📂 Drag-and-drop file input (PDF/DOCX via client-side parsing)
-   🔍 Semantic similarity visualization between chunks

🤝 Contributing
-   Pull requests and feature ideas are welcome!
-   Please keep the project lightweight and dependency-free.
-   If you submit UI changes, include a short before/after example or screenshot.

📄 License
-   This project is licensed under the MIT License.
-   You are free to use, modify, and distribute it for both personal and commercial purposes.

👨‍💻 Author
-   Developed by Ali Enver Yılmaz
-   A simple yet powerful open-source tool for developers working with RAG, LLMs, and NLP pipelines who need fast and reliable text segmentation.

🌐 Tags
-   `rag`, `text-chunker`, `nlp`, `।lm`, `embeddings`, `javascript`, `frontend-tool`, `open-source`
