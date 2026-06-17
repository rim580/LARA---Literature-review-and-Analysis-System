# LARA - Literature Analysis and Review System


## LLM-Augmented Research Assistant for Intelligent Research Paper Analysis

LARA a smart research paper assistant leverages   **Large Language Models (LLMs)** and **Retrieval-Augmented Generation (RAG)** to help users understand, summarize, and interact with research papers efficiently.

The system extracts content from academic PDFs, identifies important sections, generates section-wise summaries, and allows users to ask questions about the paper through a conversational AI interface.

The project combines **Natural Language Processing, Deep Learning, Vector Databases, and Generative AI** to reduce the time and effort required for research paper analysis.

---

#  Features

## PDF Analysis

* Upload research papers in PDF format
* Extract structured text from documents
* Detect and organize academic sections
---

##  Section-wise Summarisation

Instead of summarizing the entire paper at once, LARA generates focused summaries for individual sections to procide
* Better understanding of paper structure
* More detailed explanations
* Reduced information overload
---

##  Question Answering system

Users can interact with the uploaded paper using natural language queries.

Example questions:
* "What is the main contribution of this paper?"
* "Which dataset was used?"
* "What are the limitations of this approach?"
* "How does this method compare with existing techniques?"

The system retrieves relevant information from the paper and generates answers using an LLM.
---

#  System Architecture

```
                PDF Upload
                    |
                    ↓
          Text Extraction (PyMuPDF4LLM)
                    |
                    ↓
             Text Cleaning
                    |
                    ↓
       Section Detection & Refinement
                    |
                    ↓
              Text Chunking
                    |
                    ↓
        Embedding Generation (MiniLM)
                    |
                    ↓
          FAISS Vector Database
                    |
                    ↓
          Semantic Retrieval (MMR)
                    |
                    ↓
          LLM Response Generation
                    |
                    ↓
             Gradio Interface
```

---

# Technologies Used

| Component            | Technology                           |
| -------------------- | ------------------------------------ |
| Programming Language | Python                               |
| Frontend Interface   | Gradio                               |
| LLM                  | Llama 3.3 70B                        |
| LLM Provider         | Groq API                             |
| Framework            | LangChain                            |
| Embeddings           | all-MiniLM-L6-v2                     |
| Vector Database      | FAISS                                |
| PDF Processing       | PyMuPDF4LLM                          |
| NLP                  | Transformers / Sentence Transformers |

---

# Future Improvements

Future enhancements may include:

* Multi-paper comparison
* Citation extraction
* Research gap detection
* Knowledge graph generation
* Automatic literature review generation
* Local LLM deployment
* Hybrid search using BM25 + embeddings

---

# Author

**RIYA MATHUR**



---

# 📜 License

This project is created for educational and research purposes.


