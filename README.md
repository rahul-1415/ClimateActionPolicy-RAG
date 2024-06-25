# ClimateActionPolicy-RAG

## Overview

ClimateActionPolicy-RAG is a project focused on creating a robust retrieval-augmented generation (RAG) system to support policy recommendations for climate action. The project utilizes advanced machine learning techniques, including data cleaning, embedding generation, and a RAG system powered by Ollama's LLaMA 3 model.

## Repository Structure

- **LLM_KB.csv**: Original knowledge base for LLM before cleaning.
- **LLM_KB-DataCleaning/**: Folder containing the data cleaning scripts and relevant resources.
- **Cleaned_LLM_KB.csv**: Cleaned version of the knowledge base for LLM.
- **Reduced_LLM_KB.csv**: Reduced and optimized version of the knowledge base for faster processing.
- **Embedder.ipynb**: Jupyter notebook for generating embeddings for the knowledge base.
- **CPRAG.ipynb**: Jupyter notebook implementing the main RAG system using Ollama's LLaMA 3.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.11
- Jupyter Notebook

### Required Libraries/Packages

Install the following Python packages using pip:
```bash
  pip install pandas nltk wordcloud matplotlib chromadb langchain_community   langchain_chroma
```


### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/ClimateActionPolicy-RAG.git
    cd ClimateActionPolicy-RAG
    ```

2. Install the necessary dependencies:
  ```bash
  pip install pandas nltk wordcloud matplotlib chromadb langchain_community   langchain_chroma
  ```

### Usage

1. **Data Cleaning**:
    - Navigate to the `LLM_KB-DataCleaning` folder and run the data cleaning script:
      ```bash
      jupyter notebook LLM_KB-DataCleaning/data_cleaning.ipynb
      ```
    - This will generate the `Cleaned_LLM_KB.csv` file.

2. **Embedding Generation**:
    - Open `Embedder.ipynb` and run the notebook to generate embeddings for the cleaned knowledge base.
    - This will utilize the `Cleaned_LLM_KB.csv` and produce embeddings stored within the notebook outputs.

3. **RAG System**:
    - Open and run `CPRAG.ipynb` to implement the retrieval-augmented generation using the embeddings and the cleaned knowledge base.
    - The notebook will guide you through loading the embeddings, setting up the RAG model using Ollama's LLaMA 3, and generating policy recommendations.
