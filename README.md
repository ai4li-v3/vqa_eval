# Visual Question Answering Evaluation
Repository for automating the evaluation of Visual Question Answering (VQA) systems

## Problem Statement

Visual Question Answering (VQA) systems need thorough evaluation to determine their accuracy, reliability, and performance across various image and question types. Traditionally, evaluating VQA systems has been labor-intensive, requiring:

1. Manual review of model responses
2. Subjective judgment of answer correctness
3. Time-consuming comparison across multiple models
4. Difficulty in scaling evaluation to large datasets

This repository aims to solve these challenges by creating an automated evaluation pipeline that:

- Provides a standardized approach to evaluate multiple VQA models consistently
- Uses semantic similarity to determine answer correctness rather than exact match
- Supports multilingual evaluation capabilities
- Streamlines comparison between different model architectures (e.g., Gemini, DeepSeek, etc.)
- Generates comprehensive performance reports across different question categories and image types

Our evaluation framework leverages LiteLLM to access various models through a unified API and sentence-transformers to compute semantic similarity between predicted answers and ground truth. This approach enables more nuanced assessment of model performance beyond simple string matching.

## Features

- Unified API access to multiple AI models (Gemini, DeepSeek, etc.)
- Semantic similarity scoring using multilingual sentence embeddings
- Customizable evaluation metrics and thresholds
- Support for batch processing of test datasets
- Detailed performance reporting and visualization
