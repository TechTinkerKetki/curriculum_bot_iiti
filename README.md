# IIT Indore Curriculum Question Answering System (RAG)

## Problem Statement

IIT Indore provides curriculum information primarily through large, unstructured
PDF documents. Extracting specific details such as course syllabus, credits,
or semester-wise offerings from these documents is time-consuming and inefficient
for students.

This project aims to solve this problem by building a **Retrieval-Augmented Generation (RAG)**
based question-answering system over IIT Indore’s curriculum documents.

---

## Project Description

The system is developed using the **Computer Science (CS) curriculum of IIT Indore**
as the initial knowledge source. Users can ask natural-language questions related to
courses, syllabi, credits, and semester structures.

The system retrieves relevant sections from official curriculum documents and
generates **grounded answers** strictly based on retrieved content.

---

## Key Highlights

### Curriculum-Focused RAG Pipeline
- Designed specifically for academic curriculum documents
- Handles syllabus-heavy and table-dominant PDFs

### Smart Chunking Strategy
- Chunking is **table-centric**, not sentence-based
- Each chunk represents a meaningful academic unit (course, syllabus block, credits)
- Avoids naive row/column-count based table classification
- Preserves context required for accurate retrieval

---
## How to Use

1. Download or clone this repository
2. Open the notebooks in **Google Colab**
3. Install dependencies listed in `requirements.txt`
4. Provide your Gemini API key when prompted
5. Run the notebooks sequentially:

   ## Scope and Future Extensions

- Extend the system to include **curriculum documents from all branches**
(Mechanical, Electrical, Civil, etc.)
- Incorporate **additional IIT Indore handbooks**
(academic rules, examination manuals, hostel guidelines)
- Build a **comprehensive institutional assistant** using multiple documents
- Further improve chunking to handle:
- cross-page tables
- multi-course combined tables
- hierarchical syllabus structures
- Deploy as a full chatbot interface when infrastructure and API limits allow
