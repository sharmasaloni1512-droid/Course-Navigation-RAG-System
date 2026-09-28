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
  <img 
    src="images/rag-workflow.png" 
    alt="RAG project workflow"
    width="950"
  />
</p>





