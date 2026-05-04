# llm-rag-mastery

> **Learning RAG-based LLM application development using LangChain and Streamlit.**

This repository serves as a professional technical log for building robust, production-ready LLM applications. The primary focus is on implementing **Retrieval-Augmented Generation (RAG)** to solve real-world challenges like Hallucination and Latency, while maintaining high reliability through systematic evaluation.

---

## 🎯 Engineering Goals

Beyond basic implementation, this project focuses on the following engineering milestones:

* **Mitigating Hallucination:** Enhancing reliability by implementing source attribution (Citations) for every LLM response.
* **Optimizing User Experience:** Implementing **Streaming** responses to minimize perceived latency and improve interactivity.
* **Retrieval Refinement:** Exploring advanced data preprocessing and keyword-based retrieval to maximize search accuracy.
* **Systematic Evaluation:** Leveraging **LangSmith** to move beyond "vibe-based" testing toward data-driven performance monitoring.
* **Clean Orchestration:** Utilizing **LCEL (LangChain Expression Language)** to build modular and maintainable AI chains.

---

## 🛠 Tech Stack
* **Framework:** `LangChain` (including LCEL)
* **LLM Interface:** `OpenAI`, `Upstage`, `Ollama` (Local Environment)
* **Vector Infrastructure:** `Chroma` (Local), `Pinecone` (Cloud)
* **Frontend/Deployment:** `Streamlit`, `Streamlit Cloud`
* **Observability:** `LangSmith`

---

## 🧪 Research & Development (Experiments)

Before implementing the core logic, I conduct detailed experiments in Jupyter Notebooks to validate the performance of embedding models, retrieval accuracy, and chain behavior.

| No. | Research Topic | Description | Link | Status |
| :-- | :--- | :--- | :--- | :--- |
| 01 | **Embedding Similarity** | Testing semantic distance between words using `text-embedding-3-large`. | [Notebook](./notebooks/01_embedding_similarity_test.ipynb) | ✅ |
| 02 | **LLM Connectivity** | Validating LangChain-OpenAI integration and basic model invocation. | [Notebook](./notebooks/02_langchain_llm_validation.ipynb) | ✅ |
| 03 | **Chroma & LCEL RAG** | End-to-end RAG pipeline implementation using Chroma and LCEL. | [Notebook](./notebooks/03_rag_with_chroma_lcel.ipynb) | ✅ |
| 04 | **Manual RAG Study** | Comparative study of building RAG without LangChain to understand internal mechanics. | [Notebook](./notebooks/04_manual_rag_without_langchain.ipynb) | ✅ |
| 05 | **Pinecone & DB Migration** | Seamlessly switching from local Chroma to cloud-based Pinecone. | [Notebook](./notebooks/05_rag_with_pinecone_lcel.ipynb) | ✅ |
| 06 | **Query Transformation** | Optimizing retrieval efficiency using a Keyword Dictionary and Query Rewriting. | [Notebook](./notebooks/06_query_transformation_with_dictionary.ipynb) | ✅ |

---

## 🗺 Implementation Roadmap (WIP)

*The roadmap is subject to change based on learning progress and technical requirements.*

### Phase 1: RAG Infrastructure
- [x] **Embedding Analysis:** Understanding semantic relationships between vectors.
- [x] **Environment Setup:** Confirmed connectivity for LangChain and LLM providers.
- [x] **Vector Storage:** Implemented local persistence with **Chroma**.
- [x] **Data Pipeline:** Integrated document loading and chunking strategies.
- [x] **Framework Deep Dive:** Comparative analysis of Manual RAG vs. LangChain abstraction.

### Phase 2: Orchestration & Logic
- [x] **Chain Design:** Developed modular LLM workflows using **LCEL**.
- [x] **Multi-Vector DB:** Integrated **Pinecone** for cloud-based scaling.
- [x] **Retrieval Refinement:** Implemented **Query Transformation** using Keyword Dictionaries.

### Phase 3: Application & Evaluation
- [x] **UI/UX:** Built an interactive chat interface using **Streamlit**.
- [ ] **Integration:** Connecting the LCEL RAG Chain to the Streamlit frontend.
- [ ] **Observability:** Real-time performance tracking with **LangSmith**.

---

## 🤖 Chatbot Interface (Streamlit)
The project now features a user-centric conversational interface designed for tax-related inquiries.
*   **Session State Management:** Ensures continuity of conversation by retaining message history across re-runs.
*   **Modern Chat UI:** Implements `st.chat_message` and `st.chat_input` for a seamless, production-ready user experience.

---

## 🚀 Key Learning Focus

> "The difference between a demo and a product is reliability."

This project is not just about writing code but about understanding the **debugging process** in LLM services. It includes logs on handling API quotas, debugging chain logic, and optimizing retrieval hit rates in various environments (Cloud & Local).

---

## 👤 Author

**Park Iwan**
* Backend & AI Developer
* Focused on Agentic AI and RAG Architecture Optimization