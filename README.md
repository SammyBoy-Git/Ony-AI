# Ony AI 🤖

**Ony AI** is a lightweight, local command-line artificial intelligence terminal application written in **C++**. It integrates directly with **Ollama** (`qwen3:8b`) to provide a fully local, private, and customizable AI assistant experience right inside your Windows terminal.

---

## ✨ Key Features

* **Local & Private:** Runs entirely offline using your local Ollama instance (`qwen3:8b`).
* **Persistent Memory & Name Recognition:** Automatically saves and recalls your name (`Name.txt`) and restores your complete chat history (`Chats.TXT`) across sessions.
* **Hidden Thinking Process & Response Timers:** Keeps the model's raw reasoning trace hidden by default for a clean chat interface, recording response times down to the fraction of a second.
* **Granular Access Control:** Toggle system features like Date & Time or Internet access on the fly and store them permanently in `Setting.txt` using `(Feature) = (T/F)` format.
* **UTF-8 Encoding Support:** Cleanly renders emojis, special punctuation, and international characters in the Windows console.

---

## 📂 File & Directory Structure

Ony AI organizes its runtime assets under `C:\Projects\Ony AI`:

```text
C:\Projects\Ony AI\
│
├── AI Models\         # Ollama model manifests and files (qwen3:8b)
├── Chats\             # Session storage directory
│   ├── Name.txt       # Stores your saved user name
│   ├── Chats.TXT      # Stores complete conversation history
│   └── Setting.txt    # Stores access permissions (e.g., Date&time-access = T)
└── README.md          # Documentation file