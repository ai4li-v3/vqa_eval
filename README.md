# Visual Question Answering Evaluation
Repository for automating the evaluation of Visual Question Answering (VQA) systems

## Problem Statement

We already have a sample dataset in the `data/` folder.  
Our goal is to **automate the evaluation process**:

- For each image in the `data/image/` folder:
  - Read the corresponding label file from `data/label/`
  - Extract the question(s) and ground-truth answer(s)
  - Send a request to our model API with the image and question
  - Receive the predicted answer from the model
  - Evaluate the prediction using sentence similarity against the ground-truth answer (both in Vietnamese)

We use a similarity threshold (e.g. `0.8`) to determine whether the prediction is correct.

This process will run automatically across all samples in the dataset.



## Suggestion
We also provide [`sample.ipynb`](./sample.ipynb), which demonstrates:

1. 🔄 Using [LiteLLM](https://github.com/BerriAI/litellm) for easily switching between different models
2. 📐 Using [`sentence-transformers`](https://www.sbert.net/) to evaluate model predictions

---

## 📦 Dependency Management

We recommend using [**uv**](https://github.com/astral-sh/uv) — a fast, modern Python package manager — as it's becoming the new industry standard. However,
fell free to switch into any convenience tools of you. 


