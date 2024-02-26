# M4-Group-Assignment-3

Submitted: 28/02/2024

Created by Benjamin, Camilla and Tobias

## 1. Build a QA system that retrieves information from a given set of documents (or a document) to answer complex queries

### Document 
The document used is 'StrategicChange.pdf'

### Approach
1. **Split the documents into smaller chunks**: Splitting the document into chunks is required due to the limited number of tokens a LLM can look at once (4096 for Llama 2).
2. **Generate embeddings**: The HuggingFaceEmbeddings class is used to create embeddings for the chunks.
3. **Loading data into Chroma database**: We'll use Chroma database to store/cache the embeddings and make it easy to search them.
4. **Loading Mistral-7B-Instruct-v0.1 as LLM**: We are using Mistral-7B-Instruct-v0.1 for this question answering
5. **Implementing RAG as Q&A**

### Results
The five forces in the industry analysis are:

1. Threat of New Entrants
2. Bargaining Power of Suppliers
3. Bargaining Power of Buyers
4. Threat of Substitute Products or Services
5. Competitive Rivalry in the Industry

## 2. Develop a tool for summarizing research papers, where the system extracts key points from a database of paper vectors.

We also implemented RAG as a summarizing tool.

### Results
"Summarize the paper of Strategic Change"
