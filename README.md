# Graph RAG Project

This project demonstrates the use of Graph RAG (Retrieval Augmented Generation) by combining knowledge graphs with traditional RAG approaches. The goal is to create a more contextually aware and efficient retrieval system for generating responses from large corpora of documents.

## Introduction

Graph RAG enhances the traditional RAG system by integrating knowledge graphs, allowing for more accurate and contextually relevant responses. This approach addresses the limitations of traditional RAG, such as limited contextual understanding, scalability issues, and complexity in integrating external knowledge sources.

## Features

- **Entity and Relationship Extraction:** Automatically extract entities and relationships from documents to build a knowledge graph.
- **Knowledge Graph Creation:** Build a comprehensive knowledge graph from extracted entities and relationships.
- **Community Detection:** Group related entities into communities to enhance response generation.
- **Summarization:** Generate summaries at different levels of detail to provide a holistic understanding of the document corpus.

## Cost Considerations
Be aware that running Graph RAG, especially with models like GPT-4o, can be costly. The example in the video required over a million tokens, costing around $7. Consider the size of your corpus and the number of queries to optimize costs.

# Usage
Run a query:
python -m graphrag.query --root ./ragtest  --method global "{your question}"