    # 🚖 Multi-Turn Conversational Data Explorer (Ride Bookings)

This project implements a **multi-turn conversational agent** using **LangChain + local LLMs (Ollama)**.  
The agent can analyze a ride-booking dataset, generate visualizations, remember past context, and even engage in casual conversation.  

The project was built as part of a **Data Scientist assignment** to demonstrate skills in:  
- LLM-based agent design  
- Multi-turn context handling  
- Tool integration (data analysis + visualization)  
- Modular reasoning flow  

---

## 🎯 Objectives
The assignment required:  
- A multi-turn conversational agent with **memory**  
- At least one **tool invocation** (e.g., data analysis, web search, plotting)  
- A **structured pipeline**: Intent → Tool → Execution → Response  
- Clear documentation with setup instructions and sample interactions  

Our chosen use-case is a **Conversational Data Explorer**.  
Users can upload a CSV file (`ncr_ride_bookings.csv`) and ask questions such as:  
- *“Which vehicle type generated the most revenue?”*  
- *“Show me the revenue trend over time.”*  
- *“What is the average ride distance?”*  

---

## ⚙️ Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/your-username/multi-turn-agent.git
cd multi-turn-agent

Here's the installation and setup instructions in Markdown format:

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

**Requirements include:**
- pandas
- matplotlib
- langchain
- langchain-community
- ollama (for local LLM)

## 3. Install Ollama (for Free Local LLM)

Download and install Ollama from [ollama.ai](https://ollama.ai)

Then pull the LLaMA 3 model:

```bash
ollama pull llama3
```

## 4. Run the Agent

```bash
jupyter notebook agent.ipynb
```

## Pipeline Flow

User Query
   ↓
Intent Detection (LLM)
   ↓
Tool Selection
   ├─ If Data Query → Pandas/Matplotlib
   ├─ If Chit-Chat → LLM only
   ↓
Tool Execution
   ↓
LLM Response (polished & conversational)
   ↓
Memory Update (ConversationBufferMemory)


