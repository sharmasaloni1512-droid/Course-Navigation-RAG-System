# Course-Navigation-RAG-System
RAG based Course Navigation system for finding relevant lectures, topics and timestamp .

## Overview

> **Find the right lecture. Find the right moment. Learn faster.**
> 
It allows students to ask questions about course content and automatically finds the **relevant lecture, lecture number, video title, and timestamp** where the topic is taught.
Instead of manually searching through hours of lecture videos, users can simply ask a question and get a focused course-based answer.

## What Does It Do?
Suppose a student asks:
> Where are unordered HTML lists taught?
Instead of searching through multiple videos manually, the system retrieves the relevant course content and provides information such as:

- Lecture number
- Video title
- Relevant timestamp

This makes navigating large video-based courses faster and easier.

## Demo

> Here are some example questions and responses from the RAG system.

### Example 1 — Finding a topic in the course

**User Query**

Ask a question: Where is paragraph taught?

**Generated Response — Ollama (Llama 3.2)**

<img width="1437" height="257" alt="Generated response" src="https://github.com/user-attachments/assets/d3593b6f-f122-42ee-81d4-d063e5d43aae" />

### Example 2 

**User Query**

Ask a question: where is input tag taught in this course?

**Generated Response — Ollama (Llama 3.2)**

<img width="998" height="232" alt="Generated response" src="https://github.com/user-attachments/assets/f46ee0ce-a1fe-4695-9bbf-7af292d7e667" />

### Example 3 - a sub-topic which is taught inside the video 

**User Query**

Ask a question: Where is display property taught?

**Generated Response — Ollama (Llama 3.2)**

<img width="1422" height="366" alt="Generated response" src="https://github.com/user-attachments/assets/6319b536-9da3-4649-afa2-a8d9e0db6ce4" />

**Result:**  
The system identifies the relevant lecture, video number, and timestamp where the topic is taught.

## How It Works?

The project follows a six-step RAG pipeline, from video preprocessing
and transcription to semantic retrieval and response generation.

<p align="center">
  
  <img width="1427" height="632" alt="Screenshot 2026-09-27 232118" src="https://github.com/user-attachments/assets/ac921f39-f649-464a-a793-e90899593329" />

</p>

## Tech Stack

| Technology | Purpose |
|---|---|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) | Core development |
| ![Whisper](https://img.shields.io/badge/Whisper-412991?style=for-the-badge) | Audio transcription |
| ![BGE--M3](https://img.shields.io/badge/BGE--M3-6C5CE7?style=for-the-badge) | Text embeddings |
| ![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge) | Local LLM execution |
| ![Llama](https://img.shields.io/badge/Llama_3.2-0467DF?style=for-the-badge) | Response generation |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) | Data processing |
| ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) | Numerical operations |
| ![Scikit--learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) | Cosine similarity |
| ![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=for-the-badge&logo=ffmpeg&logoColor=white) | Video-to-audio conversion |
| ![Joblib](https://img.shields.io/badge/Joblib-4B8BBE?style=for-the-badge) | Saving processed data |

## Future Improvements

- Support multiple courses
- Add a web-based user interface
- Add clickable video timestamps
- Improve retrieval using hybrid search
- Add conversation history
- Add automatic topic summaries
- Support larger course libraries

## Why RAG?

A traditional LLM may answer course-related questions using its general
knowledge.

This project retrieves relevant information from the actual course content
and provides it to the LLM as context.

```text
User Question
      ↓
Retrieve Relevant Course Content
      ↓
Provide Context to LLM
      ↓
Generate Course-Grounded Answer

```

## Author

**Saloni Sharma**




