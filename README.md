# Loan Approval Q&A Chatbot using RAG (FAISS + LLM)

A smart Q&A chatbot that uses real loan training data, semantic search with FAISS, and a Hugging Face LLM to answer natural-language queries like:
- _"Can a female apply for a loan?"_
- _"What affects loan approval?"_

### Features
- **RAG (Retrieval-Augmented Generation)** for intelligent, data-grounded answers
- **FAISS vector search** to retrieve relevant documents from training data
- **Hugging Face models** (MiniLM + LLM like Phi-2) for question understanding and response generation
- **Gradio interface** for chat-based Q&A
- Based on real-world datasets like training, test, and sample submission CSVs

---

## Dataset Files

Make sure to include the following:
- `Training Dataset.csv`
- `Test Dataset.csv`
- `Sample_Submission.csv`

These files are used to train document embeddings and generate responses using the retrieval pipeline.

---

## Technologies Used

| Component        | Tool/Library                                |
|------------------|---------------------------------------------|
| Embeddings       | `sentence-transformers (MiniLM)`            |
| Vector DB        | `FAISS`                                     |
| Generative LLM   | `HuggingFace Transformers (e.g., Phi-2)`    |
| Interface        | `Gradio`                                    |
| Hosting          | Google Colab or Local                       |

---

## Setup Instructions

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/rag-loan-approval-chatbot
cd rag-loan-approval-chatbot

# 2. Install dependencies (Colab or local)
pip install -r requirements.txt

# 3. (Optional) Login to Hugging Face if using gated models
from huggingface_hub import login
login(token="your_HF_token")

# 4. Run the chatbot (Colab recommended)
