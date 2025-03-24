## 📄 Paper Entry

### Title: Rationalizing Neural Predictions
**Authors:** Tao Lei, Regina Barzilay and Tommi Jaakkola
**Conference/Journal + Year:** arXiv 2016
**Link:** [arXiv / OpenReview / DOI] https://arxiv.org/abs/1606.04155
**Tags:** `#NLP`

---

### 🔍 1. Summary
This paper proposes a model that simultaneously makes predictions and generates human-interpretable justifications, or rationales, from input text. These rationales are short, coherent fragments selected without supervision. 
The method uses two neural modules — a generator to select rationales and an encoder to predict labels using only the selected rationale. The model is trained end-to-end and evaluated on sentiment analysis and question retrieval tasks, 
outperforming attention-based baselines.

---

### 🧠 2. Key Ideas

Rationales: Extractive, human-readable subsets of input text sufficient for model prediction.

Generator-Encoder Framework:
- Generator: Predicts a binary mask to select words as rationales.
- Encoder: Uses only selected words to predict output.

Training Objective: Joint loss combining prediction error and regularization to encourage short, coherent rationales.

REINFORCE-style training: Because selections are discrete, the generator is trained with policy gradients.
---

### 🧪 3. Experiments & Results
1. Multi-Aspect Sentiment Analysis (BeerAdvocate dataset)

Predicts ratings for aspects like appearance, aroma, palate.
Achieves rationale precision up to 96%, far outperforming SVM (38%) and attention models (80%).

2. Similar Question Retrieval (AskUbuntu)

Extracts rationale fragments from long questions.
Outperforms full-body text representations in retrieval accuracy, achieving MAP ≈ 56% using just ~10% of text.
---

### 📊 4. Strengths

- End-to-end trainable without rationale annotations.
- Outperforms attention-based and post-hoc explanation methods.
- Modular architecture with interchangeable components.
- Applicable to both classification and retrieval tasks.

---

### ⚠️ 5. Weaknesses / Limitations
- Only supports extractive (not abstractive) rationales.
- Requires sampling (REINFORCE), which can be unstable.
- Evaluation relies on overlap with sentence-level annotations, which may be coarse.
---

### 🔗 6. Connections
- Attention models (Bahdanau et al., 2015)
- LIME (Ribeiro et al., 2016) — post-hoc explanations
- Rationale-augmented CNNs (Zaidan et al., 2007; Zhang et al., 2016)
---

### 💡 7. Thoughts & Questions
- Could this be extended to abstractive rationales using generative models?
- Apply to other domains like clinical NLP, legal text, fact-checking?
- Add human evaluation of rationale quality for trust and usability.
---
