# Extracting and Reconstructing Knowledge in Material Science Literature Using Large Language Models
#Overview
This project provides a generalized framework for reconstructing knowledge from inorganic materials science literature using advanced large language models (LLMs). The goal is to accelerate materials discovery by enabling large-scale, accurate, and consistent extraction of synthetic routes, properties, and other valuable scientific information from published articles.

One-Prompt Knowledge Reconstruction: Constructs the dataset using a one-shot prompt approach combined with human feedback, ensuring data quality for model training and fine-tuning.
Multi-Model Fine-Tuning: Four models—LLaMA3-8B-instruct, Gemma-7B, Phi3-mini-128k-instruct, and GPT3.5-turbo-1106—were fine-tuned using the generated dataset.
High Extraction Accuracy: Achieved precision of 0.928, recall of 0.957, and F1-score of 0.962 in extracting synthetic procedures for selective catalytic reduction.
Scalable Extraction Workflow: Extracted nearly 49,000 entities from over 2,200 materials science articles, saving results in structured JSON files.
Cross-Domain Transferability: Fine-tuned models were successfully applied to five additional domains (lithium-ion batteries, hydrogen evolution reaction, etc.), showing strong generalization across materials science tasks.
Knowledge Graph Construction: Integrates extracted metadata, catalysts, preparation details, synthesis conditions, and performance into a knowledge graph.
