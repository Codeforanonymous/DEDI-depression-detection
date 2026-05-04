
**Listening to the Quiet Grief: The Depression Emotion Disproportion Index (DEDI) for Depression Risk Assessment**

This repository contains the experimental code for the paper *"Listening to the Quiet Grief: The Depression Emotion Disproportion Index (DEDI) for Depression Risk Assessment"*. It is provided for reviewers to facilitate reproducibility and verification of results.

## Key Contributions

- **DEDI (Depression Emotion Disproportion Index)**: A novel user-level metric quantifying the relative dominance of depression-linked emotions (sadness, grief, remorse, disappointment, disapproval) based on the GoEmotions taxonomy.
- Multimodal BERT-based model fusing contextual embeddings, TF-IDF features, and subreddit embeddings.
- Rigorous **length-matched** evaluation to control for posting volume and text length confounds.
- Comprehensive experiments across realistic prevalence rates: **5.00%**, **11.02%**, and **15.00%**.

## Core Notebooks

| Notebook | Description | Paper Sections |
|---------|-------------|----------------|
| `01_Emotion_Distribution.ipynb` | Data preprocessing | Section 3, Figure 1 |
| `02_Baselines.ipynb` | All baseline models (TF-IDF + LR/SVM/RF, CountVectorizer, Vanilla BERT, Subreddit-only) | Section 4.3, Table 2 |
| `03_Main_Models.ipynb` | Main multimodal model training, length-matched evaluation across multiple prevalences, error analysis, and publication-ready figures | Sections 4–6, Table 1, All Figures |


Hardware Recommendation

GPU recommended (≥8GB VRAM) for faster BERT training and inference.
Experiments can run on CPU but will be significantly slower.
