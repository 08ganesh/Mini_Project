# Mini_Project
#  Extractive Text Summarization using LLMs and Hierarchical Positional Encoding

---

##  Project Overview

This project presents a **semantic-driven extractive summarization framework** that improves the summarization of long-form documents by combining **Large Language Models (LLMs)** like **MPNet** with **Hierarchical Positional Encoding (HPE)**. It identifies the most relevant, coherent, and novel sentences from complex documents using structural parsing, semantic clustering, and multi-factor scoring.

---

##  Authors

- **Eggoni Ganesh** 
- **Gaddapara Manohar**
- **Kamanuru Ajay Krishna**  



---

##  Key Objectives

- Enhance extractive summarization of complex documents using semantic embeddings.
- Capture the document’s **hierarchical structure** through tree-based modeling.
- Minimize **redundancy** and maximize **coherence, novelty, and relevance** in summaries.
- Outperform traditional models like LexRank and PEGASUS in ROUGE metrics.

---

##  System Architecture

The project follows an **8-stage pipeline**:

1. **Data Collection**: Long-form documents from datasets like CNN/DailyMail  
2. **Preprocessing & Structural Parsing**: Sentence tokenization + semantic sectioning  
3. **Hierarchical Tree Construction**: Nodes represent paragraphs, headers, sentences  
4. **Triplet Positional Encoding**: Encodes node depth, position & contextual importance  
5. **Contextual Relevance Scoring**: Measures how well a sentence represents the document  
6. **Semantic Clustering & Selection**: Picks representative sentences from clusters  
7. **Refinement & Redundancy Removal**: Enhances fluency and removes duplication  
8. **Evaluation**: Uses ROUGE-1, ROUGE-2, and ROUGE-L to compare with baselines

---

##  Tech Stack

- **Language**: Python 3.8+
- **Frameworks & Libraries**:  
  - PyTorch  
  - HuggingFace Transformers  
  - Scikit-learn  
  - NLTK  
  - NumPy, Pandas  
  - ROUGE Toolkit  
  - Matplotlib / Seaborn for visualizations
- **Platforms**: Google Colab / VS Code / Jupyter  
- **OS Compatibility**: Ubuntu 20.04 LTS or Windows 10+

---

##  Evaluation Metrics

Summaries were evaluated using ROUGE scores:

| Metric    | Description                                  |
|-----------|----------------------------------------------|
| ROUGE-1   | Unigram (word-level) overlap                 |
| ROUGE-2   | Bigram (phrase-level) overlap                |
| ROUGE-L   | Longest common subsequence (structural flow) |

Our model demonstrated **notable improvements** compared to LexRank and PEGASUS, particularly in recall-oriented evaluation.

---

##  Strengths

- Semantic sentence understanding with **MPNet embeddings**
- Structure-aware summarization via **hierarchical trees**
- Enhanced **triplet positional encoding** (depth, position, importance)
- Multi-dimensional scoring: relevance, coherence, novelty, redundancy
- Strong performance on benchmark datasets (ROUGE-based)

---

##  Limitations

- Requires **high computational resources** (GPU, RAM)
- Purely extractive – lacks abstraction or paraphrasing
- Not optimized for **real-time** or **low-resource** deployment
- Multi-stage design increases implementation complexity

---

##  Future Enhancements

- Integrate **abstractive summarization** for hybrid results
- Use **smaller/faster models** for edge deployment
- Expand support for **multilingual summarization**
- Introduce **interactive/customizable summarization**
- Apply to **streaming data** or **live conversations**

---
