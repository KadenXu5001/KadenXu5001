
# 👋 Hey there, I'm Kaden!

## 🚀 About Me

```python
from langchain.agents import initialize_agent, AgentType
from langchain.llm import Kaden 
from langchain.tools import Tool


tools = [
    Tool(
        name="Python",
        description="Snake go Brrrrr"
    ),
    Tool(
        name="AI",
        description="Millions must eval()"
    ),
    Tool(
        name="Teamwork",
        description="1 + 1 > 1"
    )
]

llm = Kaden(temperature=67)

agent_kwargs = {
    "prefix": "You are an AI agent with the following traits:\n"
              "- Optimistic\n"
              "- Comfy\n",
              "- Always Learning\n",
    "suffix": "I said No mistakes 😠"
}

agent = initialize_agent(
    tools,
    llm,
    agent=AgentType.TRUST_THE_PROCESS,
    agent_kwargs=agent_kwargs,
    verbose=any(topic in question for topic in ["Tetris", "Chess", "Fantasy Football"])
)


result = agent.run("Pleasure to meet you!")
```



## ⭐ Featured Projects

### Finetuned Reddit Discourse Model
**Tech:** Python, DistilBERT, PowerBI, Groq | [Video Demo](https://youtu.be/dJdEA7gAo7c) | [Github](https://github.com/KadenXu5001/TakeMaker)

Hand-annotated 200+ R/nba posts to fine-tune a DistilBERT text classifier for discourse quality evaluation. Achieved **86.8% accuracy** and **0.906 macro F1**, outperforming LLaMA-3.3-70B by **36.8%**.

### Vector-Based Music Recommendation System
**Tech:** React, Cohere, Docker, FastAPI | [Website](https://Algorythems.com) | [Video Demo](https://youtu.be/uq_ifn57EWM) | [Github](https://github.com/KadenXu5001/Algorythem)

Deployed an ML-powered song recommendation system on AWS Lightsail, indexing 500+ tracks via a RAG pipeline using embedded Whisper transcripts and CLAP audio features stored in Pinecone vector database.

### Edge-AI Wearable Gesture Scrolling
**Tech:** Scikit-learn, PyTorch, CircuitPython, BLE | [Video Demo](https://youtube.com/shorts/W0R-ZdRyBGk?feature=share) | [Github](https://github.com/danielshamsoddini/CS396-ML-Sensing-Final-Project)

Real-time sensor-informed pipeline for YouTube Shorts navigation. Trained SVM and MLP classifiers on 6 gesture classes, achieving **95.6% F1-score**.

### Intelligent Receipt Processing System
**Tech:** Java, Spring Boot, React, Supabase, Jira | [Video Demo](https://youtu.be/MWY155FZIDA) | [Github](https://github.com/CS-396-Full-Stack-Software-Eng/final-project-divide-and-concur)

Full-stack expense platform with OCR agent for receipt scanning. Built with Next.js, Spring Boot, Redis/WebSockets, and GraphQL—cutting item-claiming time by **65%**.
