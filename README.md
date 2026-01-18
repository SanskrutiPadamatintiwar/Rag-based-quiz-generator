# RAG-Based Quiz Generator 🧠

A full-stack application that generates quizzes using a Retrieval-Augmented Generation (RAG) pipeline.  
The system accepts a user-defined topic and optional documents, builds a knowledge base, and uses an LLM to generate quiz questions.

---

## Overview

This project demonstrates how RAG can be applied to generate meaningful quiz questions from both user-provided content and trusted external sources.

If documents are not provided, the system retrieves relevant information from a predefined set of trusted resources to construct the knowledge base before quiz generation.

---

## Key Features

- Topic-based quiz generation  
- Document ingestion for custom knowledge bases  
- Automatic retrieval from trusted sources when documents are absent  
- RAG pipeline for grounded question generation  
- Multiple question types:
  - Multiple Choice Questions (MCQs)
  - Fill-in-the-Blanks  
- JWT-based authentication  
- Clean separation of frontend and backend  

---

## Tech Stack

### Frontend
- React

### Backend
- FastAPI (Python)

### AI / ML
- Retrieval-Augmented Generation (RAG)
- Microsoft Phi-3.5 LLM

### Auth & Security
- JWT-based authentication

---

## How It Works

1. User provides a topic and optional reference documents  
2. If documents are missing, the system retrieves relevant content from trusted sources  
3. A knowledge base is constructed from the collected data  
4. The RAG pipeline feeds relevant context to the LLM  
5. The LLM generates quiz questions grounded in the retrieved knowledge  

---

## Project Structure

```

/frontend      # React frontend
/backend       # FastAPI backend
/auth          # JWT authentication logic
/rag           # Retrieval and generation pipeline

````

*(Structure may vary slightly based on configuration.)*

---

## Setup (Local)

```bash
git clone https://github.com/SanskrutiPadamatintiwar/rag-based-quiz-generator.git
cd rag-based-quiz-generator
````

### Backend

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend

```bash
cd frontend
npm install
npm start
```

---

## Use Cases

* Educational platforms
* Personalized learning tools
* Interview preparation systems
* Knowledge assessment applications

---

## Future Improvements

* Quiz difficulty tuning
* User performance analytics
* More question formats
* Improved retrieval ranking
* Production deployment with CI/CD

---

## Why This Project

This project was built to explore real-world usage of RAG systems beyond demos, focusing on:

* grounding LLM outputs with reliable context
* backend–frontend integration
* secure APIs and extensible architecture

---

## Author

Sanskruti Padamatintiwar

