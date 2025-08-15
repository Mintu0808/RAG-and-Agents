# Knowledge Process Repository
This repository contains theoretical and practical content related to:
- **Retrieval-Augmented Generation (RAG)**
- **AI Agents**
- **Agentic AI**

The goal is to provide a central knowledge hub combining concepts, workflows, and example implementations.

---

## 📌 Retrieval-Augmented Generation (RAG)

### 1. What is RAG?
Retrieval-Augmented Generation (RAG) is a technique that combines **information retrieval** and **text generation** to produce more accurate, context-aware, and up-to-date responses from Large Language Models (LLMs).  
Instead of relying solely on the LLM's pre-trained knowledge, RAG retrieves relevant documents from an **external knowledge source** (e.g., vector database, search index) and feeds them into the model as context.

---

### 2. Why RAG?
- **Factual accuracy** → reduces hallucinations by grounding outputs in retrieved facts.
- **Fresh knowledge** → can use the most recent data, even beyond the LLM's training cut-off.
- **Domain-specific customization** → tailor outputs using your own proprietary datasets.
- **Smaller models can act smarter** → retrieval compensates for limited parameters.

---

### 3. How RAG Works
1. **Query** → User asks a question or makes a request.
2. **Retrieve** → Search for relevant documents in an external data store (vector DB, Elasticsearch, Azure Cognitive Search, etc.).
3. **Augment** → Add the retrieved documents to the LLM’s input prompt.
4. **Generate** → LLM uses both its training + the retrieved content to produce a final answer.

**Workflow Diagram:**
![RAG Workflow](assests/rag_workflow_diagram.png)
