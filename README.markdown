# Ride Booking Data Assistant

A simple conversational agent for analyzing ride booking data using local LLMs with LangChain and Ollama.

## 🎯 What It Does

- Answers questions about ride booking data in plain English
- Generates simple charts and visualizations
- Maintains conversation history
- Runs offline with local AI models

## ⚙️ Setup

### 1. Clone Repository
```bash
git clone https://github.com/Nooby-Sandwich/multi-turn-agent.git
cd multi-turn-agent
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

**Requirements:**
- pandas
- matplotlib
- langchain
- langchain-community
- ollama (for local LLM)

### 3. Install Ollama
Download and install Ollama from [ollama.ai](https://ollama.ai)

Pull the LLaMA 3 model:
```bash
ollama pull llama3
```

### 4. Run the Agent
```bash
jupyter notebook agent.ipynb
```

## 💬 Example Questions

- "Which vehicle type earned the most?"
- "Show revenue over time"
- "Average ride distance?"
- "Bookings per day?"

## 🔄 How It Works

1. Ask a question about the data
2. System processes the request
3. Retrieves data or creates charts
4. Provides an answer
5. Remembers conversation context