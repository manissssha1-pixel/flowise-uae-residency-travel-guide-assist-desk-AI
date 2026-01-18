# UAE Residency and Travel Guide Assist Desk AI

**UAE Residency and Travel Guide Assist Desk AI** is an intelligent AI assistant built with Flowise that provides accurate, context-aware answers to queries about UAE residency, visa regulations, entry and residency schemes, destination guidance, health conditions, and common challenges faced by residents or travelers. It leverages LLMs, embeddings, and vector search to retrieve relevant information efficiently from large document collections.

---

## Features

- Answer questions related to **UAE residency visas, entry/residency schemes, and regulations**  
- Provide guidance on **health conditions, healthcare, and safety** in the UAE  
- Offer **destination guidance**, tips, and common challenges for residents and travelers  
- Maintain **context across multi-turn conversations**  
- Retrieve information from large document collections using **semantic search**  

---

## Flowise Project Architecture

This project uses **five key Flowise nodes**:

1. **Chat OpenAI**  
   - Generates conversational AI responses to user queries  
   - Provides professional and human-readable answers  

2. **Conversation Summary Buffer Memory**  
   - Maintains conversation context for multi-turn dialogues  
   - Ensures the assistant can follow up on previous questions  

3. **OpenAI Embeddings**  
   - Converts documents and user queries into vector representations  
   - Enables semantic search for accurate retrieval  

4. **Conversational Retriever QA Chain**  
   - Combines embeddings with LLM reasoning to retrieve relevant information  
   - Ensures answers are context-aware and based on UAE-specific documents  

5. **Pinecone**  
   - Vector database to store document embeddings  
   - Provides fast similarity search to retrieve the most relevant content  

---

## How It Works

1. **User Query** → Input into Chat OpenAI node  
2. **Memory Node** → Conversation Summary Buffer Memory keeps context  
3. **Embedding Node** → OpenAI Embeddings converts documents and queries to vectors  
4. **Retriever Node** → Conversational Retriever QA Chain searches Pinecone for UAE-specific information  
5. **Response Generation** → Chat OpenAI generates professional, context-aware answers  

---

## Tech Stack

- **Flowise** – Node-based workflow orchestration  
- **OpenAI / ChatGPT** – Conversational AI and reasoning  
- **OpenAI Embeddings** – Semantic representation of documents and queries  
- **Pinecone** – Vector database for fast similarity search  
- **Conversational Memory** – Maintains context for multi-turn queries  

---

## Installation & Setup

1. **Clone the repository:**

```bash
git clone https://github.com/manissssha1-pixel/flowise-uae-residency-travel-guide-assist-desk-AI
