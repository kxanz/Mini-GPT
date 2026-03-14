# Nano-GPT: Character-Level Shakespeare Generator

This repository contains a from-scratch implementation of a **Transformer Decoder**, following the architecture that powers modern LLMs like GPT-4. 

## 🔬 Architecture Overview
The model is a character-level language model that predicts the next character in a sequence based on a context of 32 previous characters.

### Key Components:
* **Multi-Head Self-Attention:** Parallel "heads" that allow the model to focus on different parts of the text simultaneously.
* **Causal Masking:** A triangular mask that prevents the model from "looking into the future" during training.
* **Residual Connections & LayerNorm:** Architectural choices that prevent vanishing gradients and allow for deeper networks.

## 🛠️ Hyperparameters
- **Batch Size:** 16
- **Block Size (Context):** 32
- **Embedding Dimension:** 64
- **Attention Heads:** 4
- **Layers:** 4
- **Dropout:** 0.0 (No regularization for this small scale)
