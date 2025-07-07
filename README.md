# Extracting and Reconstructing Knowledge in Material Science Literature Using Large Language Models
Overview：
This project provides a generalized framework for reconstructing knowledge from inorganic materials science literature using advanced large language models (LLMs). The goal is to accelerate materials discovery by enabling large-scale, accurate, and consistent extraction of synthetic routes, properties, and other valuable scientific information from published articles.

One-Prompt Knowledge Reconstruction: Constructs the dataset using a one-shot prompt approach（prompt.txt）combined with human feedback, ensuring data quality for model training and fine-tuning

LLMs Fine-Tuning: Four models—LLaMA3-8B-instruct, Gemma-7B, Phi3-mini-128k-instruct, and GPT3.5-turbo-1106—were fine-tuned using the generated dataset.（“Fine-tuning data set.jsonl”）

High Extraction Accuracy: Achieved precision of 0.928, recall of 0.957, and F1-score of 0.962 in extracting synthetic procedures for selective catalytic reduction.

Scalable Extraction Workflow: Extracted nearly 50,000 entities from materials science articles, saving results in structured JSON files.（ “Extracted information .zip”）

Cross-Domain Transferability: Fine-tuned models were successfully applied to five additional domains (lithium-ion batteries, hydrogen evolution reaction, etc.), showing strong generalization across materials science tasks.

Knowledge Graph Construction: Integrates extracted metadata, catalysts, preparation details, synthesis conditions, and performance into a knowledge graph.（“KG-rels.xlsx”）

Requirements：
Hardware
NVIDIA RTX 4090 GPU server (or equivalent, for model fine-tuning and large-scale inference)
At least 24 GB system RAM recommended
Python 3.8+
CUDA support
Transformers
OpenAI API access (for GPT-4/GPT-3.5 data generation)
Neo4j database (for knowledge graph storage and querying)

Accounts & Cloud Services
Valid OpenAI API key (for prompt-based data generation and inference with OpenAI models)
Access credentials for your Neo4j database instance

Output：
Extracted information (entities, synthesis steps, properties) will be stored in JSON format in the folder of “Extracted information .zip”.
A knowledge graph (e.g., .（“KG-rels.xlsx”）) can be constructed for downstream analysis.

Citation
If you use this code or data in your research, please cite:
article{
  title={Extracting and Reconstructing Knowledge in Material Science Literature Using Large Language Models},
  author={Shuyuan Li, Shihao Wei，Chenyu Huang，Yunjiang Zhang，Guizhen Zhang* and Shaorui Sun*},
  year={2025}
}


For questions or contributions, please open an issue or contact sunsr@bjut.edu.cn

