# Legal RAG Question Answering System

## Project Overview
This project implements a Retrieval-Augmented Generation (RAG) system to answer legal questions in a simple and understandable way.

The system retrieves relevant legal texts and uses a language model to generate clear answers based on this context.

---

## Objective
- Build a RAG pipeline using:
  - ChromaDB (vector database)
  - Hugging Face LLM (flan-t5)
- Provide accurate, context-based answers to legal questions

---

## Dataset
Source: Kaggle  
The dataset contains :
- Original legal texts  
- Simplified explanations  

This structure helps the model generate accurate and easy-to-understand answers.

---

## Methodology
The system follows these steps:
1. Data preparation (build documents)
2. Text chunking
3. Embedding generation (Sentence Transformers)
4. Storage in ChromaDB
5. Retrieval of relevant documents
6. Prompt construction
7. Answer generation using LLM

---

## Models Used
- Embedding model: all-MiniLM-L6-v2  
- LLMs:
  - flan-t5-base  
  - flan-t5-large  

---

## 🧪 Experiments
- Model comparison:
  - flan-t5-base vs flan-t5-large  
  - Result: similar answers, large model slower  

- Prompt comparison:
  - Basic prompt  
  - Simplified prompt  
  - Strict prompt  
  - Result: prompt affects answer style and safety  

---

## Results
- The system generates relevant and understandable answers  
- Some answers are short or similar due to similar retrieved context  

---

## Limitations
- Small dataset → limited diversity  
- Similar documents → repeated answers  
- No complex reasoning  

---

## Future Improvements
- Use larger datasets  
- Improve retrieval quality  
- Use more powerful models  
- Add conversational memory  

---

## Interface
A simple Gradio interface allowing users to ask questions and receive answers.

## 👤 Author
Selina Zoabi
