# ⬡ CrewAI GenAI Research Studio

> A **multi-agent AI pipeline** that researches, writes, and reviews technical content on any AI topic — powered by **CrewAI** + **Gemini 2.5 Flash**, with a polished **Gradio** frontend.

---



## 🧠 How It Works

Three specialised AI agents collaborate in sequence:

```
User Topic ──▶ 🔍 AI Researcher ──▶ ✍️ Technical Writer ──▶ ✅ AI Reviewer ──▶ Workshop Content
```

| Agent | Role | Output |
|-------|------|--------|
| **AI Researcher** | Finds 2025 trends in LLMs, Agentic AI, frameworks & enterprise adoption | Bullet-point research summary |
| **Technical Writer** | Converts research into structured, jargon-free technical content | Headed article with bullet points |
| **AI Reviewer** | Checks accuracy, clarity, flow & workshop suitability | Final polished content |

---

## 📦 Tech Stack

| Layer | Technology |
|-------|-----------|
| Agent Orchestration | [CrewAI](https://crewai.com) |
| LLM | Gemini 2.5 Flash via `langchain-google-genai` |
| Frontend | [Gradio](https://gradio.app) |
| Language | Python 3.10+ |

---

## 🛠️ Installation

```bash
# 1. Clone the repo
git clone https://github.com/your-username/crewai-research-studio.git
cd crewai-research-studio

# 2. Create a virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install crewai gradio langchain-google-genai
```

---

## ⚡ Usage

```bash
python app.py
```

Then open `http://localhost:7860` in your browser.

### Steps:
1. Paste your **Google API Key** (get one at [aistudio.google.com](https://aistudio.google.com))
2. Enter a **research topic** (default: *Generative AI and Agentic AI*)
3. Adjust **temperature** (0 = focused, 1 = creative)
4. Click **▶ Run Crew** and wait ~1–3 minutes

---

## 🗂️ Project Structure

```
crewai-research-studio/
├── app.py              # Gradio UI + CrewAI pipeline
├── requirements.txt    # Python dependencies
└── README.md
```

---

## 📋 Requirements

```txt
crewai>=0.28.0
gradio>=4.0.0
langchain-google-genai>=1.0.0
```

---

## 🔑 Environment Variables

| Variable | Description |
|----------|-------------|
| `GOOGLE_API_KEY` | Your Google AI Studio API key |

You can also set it via the UI directly — no `.env` file needed.

---

## 💡 Customisation Ideas

- 🔧 Swap Gemini for **OpenAI GPT-4o** or **Anthropic Claude** by changing the `LLM` config
- 📝 Add a **4th agent** (e.g. a LinkedIn Post Writer or Slide Deck Creator)
- 🌐 Enable **web search tools** for real-time data retrieval
- 💾 Add **file export** (Markdown / PDF) to download the final report

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

