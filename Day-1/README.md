
# Day 1 – Understanding AI Context, Learning, Hallucination and RAG

## Overview

Today we learned the basic concepts behind how AI language models process information and generate responses.

## What We Learned

### Context Window

A context window is the amount of information an AI model can process during a single call.

It can contain the system instructions, conversation history, user input, provided documents, and the generated response.

All this information must fit within the available context window.

### Self-Supervised Learning

We learned that language models can learn using self-supervised learning.

The model learns patterns from large amounts of text by predicting missing or next parts of the text.

This helps the model learn language structure, grammar, relationships between words, and common patterns.

### Hallucination

Hallucination occurs when an AI model produces information that sounds correct or confident but is incorrect or unsupported.

The model generates likely and meaningful text, but it does not automatically verify that every statement is true.

### Context and Accuracy

Providing relevant and reliable information to the model at question time can help it generate more grounded responses.

### Retrieval-Augmented Generation (RAG)

RAG stands for Retrieval-Augmented Generation.

It retrieves relevant information and provides it to the AI model as context before generating a response.

RAG can help improve the relevance and reliability of responses and reduce hallucination.

RAG does not retrain the AI model. It provides additional information during the answering process.

## Key Takeaways

- AI models have a limited context window.
- Self-supervised learning helps models learn from large amounts of text.
- AI models can sometimes produce hallucinated information.
- Relevant context can help improve AI responses.
- RAG connects AI models with external information.
- RAG provides information at question time instead of retraining the model.
