# Trust-Aware Retrieval-Augmented Generation (Trust-RAG)

## Project Title
**Trust-Aware Retrieval-Augmented Foundation Models with Adaptive Evidence Weighting and Selective Abstention for Domain-Specific Grounded Generation**

## Project Overview
This project implements a Trust-Aware Retrieval-Augmented Generation (Trust-RAG) framework to improve the reliability of AI-generated answers. Standard RAG systems retrieve documents and generate answers, but they may still produce incorrect or unsupported responses when the retrieved evidence is noisy, irrelevant, incomplete, or conflicting.

The proposed Trust-RAG framework improves standard RAG by adding:
- Adaptive evidence weighting
- Faithfulness verification
- Uncertainty calibration
- Selective abstention
- Robustness evaluation
- Efficiency and latency analysis

The main goal is to reduce hallucination and improve evidence-supported answer generation.

---

## Research Aim
The aim of this project is to design and evaluate a Trust-Aware RAG framework that produces more reliable, evidence-supported, and confidence-aware answers compared with a Vanilla LLM and Standard RAG baseline.

---

## Research Questions
The project is organized around seven research questions:

1. **RQ1:** How does Trust-RAG improve answer correctness and reduce hallucination compared with Standard RAG and Vanilla LLMs?
2. **RQ2:** How effectively does adaptive evidence weighting improve retrieval reliability under noisy or conflicting retrieval conditions?
3. **RQ3:** To what extent does faithfulness verification improve alignment between generated answers and supporting evidence?
4. **RQ4:** How well does uncertainty estimation align predicted confidence with actual answer correctness?
5. **RQ5:** Can selective abstention reduce incorrect responses while maintaining acceptable answer coverage?
6. **RQ6:** How robust is Trust-RAG under noisy, incomplete, and adversarial retrieval conditions?
7. **RQ7:** What is the computational overhead of Trust-RAG compared with Standard RAG?

---

## Dataset
The primary dataset used in this project is:

- **SQuAD v2**
- https://www.kaggle.com/datasets/thedevastator/squad2-0-a-challenge-for-question-answering-syst

SQuAD v2 provides question, context, and answer triples, making it suitable for evaluating question-answering and retrieval-augmented generation systems.

The retrieval corpus is built using SQuAD v2 context passages.

---

## Tools and Libraries
The project is implemented in Python using Kaggle notebooks.

Main tools and libraries include:

- Python
- Kaggle Notebook Environment
- PyTorch
- Hugging Face Transformers
- sentence-transformers
- FAISS
- pandas
- NumPy
- scikit-learn
- matplotlib

---

## Models Used

### Embedding Model
```text
sentence-transformers/all-MiniLM-L6-v2
