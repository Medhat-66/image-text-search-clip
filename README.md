# Image-Text Search Engine — CLIP

A multimodal image search engine that retrieves images using natural language queries, built with OpenAI's CLIP model.

## Results

| Metric | Score |
|---|---|
| Recall@1 | 72.00% |
| Recall@5 | 95.50% |
| Recall@10 | 98.50% |

## Dataset
- MS COCO 2017 — Kaggle
- 200 images with captions

## How it Works
1. CLIP encodes all images into 512-dim feature vectors
2. User enters a text query
3. CLIP encodes the query into the same feature space
4. Cosine similarity finds the most relevant images

## Model
- **Architecture:** CLIP ViT-B/32 (OpenAI)
- **Parameters:** 151,277,313
- **Embedding Size:** 512 dimensions

## Steps Performed
- **EDA:** Caption length distribution, most common words analysis
- **Feature Extraction:** CLIP image embeddings for 200 images
- **Search Engine:** Cosine similarity between text and image features
- **Evaluation:** Recall@1, Recall@5, Recall@10
- **Deployment:** Streamlit interactive web application

## Libraries
Python, PyTorch, OpenAI CLIP, Streamlit, HuggingFace Datasets, Matplotlib, NumPy
