# Agentic RAG: Turbocharge Retrieval-Augmented Generation with Query Reformulation and Self-Query

This project demonstrates how to enhance **Retrieval-Augmented Generation (RAG)** pipelines by integrating **query reformulation** and **self-query techniques** using agent-based reasoning. The goal is to improve retrieval quality and response relevance by allowing language models to actively participate in the query refinement process.

## What is RAG?

**RAG** refers to using a Large Language Model (LLM) to answer a user query by retrieving relevant documents from a knowledge base and grounding the response on that information.

### Advantages of RAG:

* Reduces hallucinations by grounding answers in retrieved data
* Enables domain-specific augmentation without retraining the LLM
* Offers granular control over information access

## Key Components

### 1. Environment Setup

The notebook includes:

* Installation of required libraries
* Initialization of the runtime environment (e.g., GPU support)

### 2. Dataset Handling

* Loads a custom dataset relevant to the use case
* Preprocesses and embeds the data
* Stores vectors into a vector database for fast retrieval

### 3. Agentic RAG Architecture

* **RetrieverTool**: A custom tool to search the vector store
* **Agent Creation**: Uses tools and an LLM to perform iterative query reformulation
* **Self-Querying**: The agent refines its own queries before retrieving information


## Evaluation

The notebook compares standard RAG with the proposed **Agentic RAG**, analyzing:

* Retrieval accuracy
* Answer relevance
* Responsiveness to complex user queries


## Project Structure

```bash
.
├── Agentic_RAG_turbocharge_RAG_with_query_reformulation_and_self_query.ipynb
├── README.md
```


## Getting Started

### Prerequisites

Ensure the following Python packages are installed:

```bash
langchain
openai
faiss-cpu
tqdm
datasets
```

### Running the Notebook

Open the notebook in Google Colab or Jupyter and follow the step-by-step cells. Ensure a GPU runtime for faster execution.


## Future Work

* Integration with real-time document updates
* Expansion to multimodal datasets
* Deploying as a web-based RAG assistant


## License

This project is for educational and research purposes.
