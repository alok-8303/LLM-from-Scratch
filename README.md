# 🚀 Building GPT-2 from Scratch

This repository contains my implementation of the GPT-2 language model built from scratch, inspired by Sebastian Raschka's book "Build LLM from Scratch".

## 📌 Overview

This project walks through the process of building a GPT-2 style language model from first principles. It's designed to be educational, showing the step-by-step implementation of a transformer-based language model without relying on high-level abstractions from frameworks like PyTorch.Also used open ai pre-trained weights for classification.

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- PyTorch 1.9+
- CUDA-capable GPU (recommended for faster training)

### Installation

```bash
# Clone this repository
git clone https://github.com/alok-8303/LLM-from-Scratch.git
cd LLM-from-Scratch

# Create and activate a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```
I have implemented this book in google collab so for importing functions there is a file gpt.py(for all ch 1-5 functions used). 

## 🔍 Features

- **Transformer Architecture**: Complete implementation of the transformer architecture that powers GPT-2
- **Multi-Head Attention**: From-scratch implementation of the attention mechanism
- **Tokenization**: Custom tokenizer implementation
- **Training Pipeline**: Full training loop with gradient accumulation and checkpointing
- **Text Generation**: Methods for generating text using the trained model
- **Poem Classification**: Implementation of the poem classification task (Chapter 6)

## 🧠 Implementation Details

This implementation focuses on the core components of the GPT-2 architecture:

1. **Tokenization**: Converting text to token IDs
2. **Positional Encoding**: Adding position information to tokens
3. **Self-Attention**: The mechanism that allows the model to focus on different parts of the input
4. **Feed-Forward Networks**: Processing representations from the attention layer
5. **Layer Normalization**: Stabilizing training by normalizing activations
6. **Masked Training**: Training the model to predict the next token

## 📊 Poem Classification Task

I've implemented the poem classification task from Chapter 6, which classifies poems into these categories:
- Arts & Sciences
- Nature
- Religion
- Relationships
- Love

The implementation can be found in the `Chapter6/poem_classification` directory.

## 📋 TODO

- [ ] Implement beam search for better text generation
- [ ] Add parameter-efficient fine-tuning options
- [ ] Experiment with different positional encoding methods
- [ ] Integrate quantization for model compression
- [ ] Implement AI agent capabilities

## 📚 Resources

- Sebastian Raschka's "Build LLM from Scratch" book
- [Github repository of book](https://github.com/rasbt/LLMs-from-scratch)

## 🙏 Acknowledgments

Special thanks to Sebastian Raschka for his excellent book that made this implementation possible.

