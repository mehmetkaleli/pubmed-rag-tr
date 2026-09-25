# Pubmed-RAG-TR Research Notebooks

This codebase is a part of a manuscript submission for `PeerJ Computer Science`.

Manuscript Title: `Enhancing multilingual retrieval-augmented-generation systems: bridging the gap for Turkish language and medical domain applications`

Link to datasets:
Translated dataset: https://huggingface.co/datasets/SMARTICT/Pubmed-RAG-TR

Eval dataset: https://huggingface.co/datasets/SMARTICT/Pubmed-RAG-TR-LLM-Eval

1. `01_data_and_model_provenance.ipynb` — loads the two public Hugging Face datasets, validates their schemas, reproduces the dataset-quality summary, records the exact evaluation split, and documents/prepares the embedding and reranker training inputs.
2. `02_rag_evaluation_and_beir.ipynb` — implements the RAG configurations, reciprocal-rank fusion, text/RAGAS metrics, paired significance tests, and the BEIR-style retrieval benchmark.

Both notebooks are self-contained and use repository-relative output paths. Expensive model training, generation, RAGAS judging, and full retrieval benchmarking are disabled by default behind clearly named `RUN_*` switches. No credentials are stored in the notebooks; optional API stages read `GOOGLE_API_KEY`, `OPENAI_API_KEY`, and `HF_TOKEN` from the environment.

