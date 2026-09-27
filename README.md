# MiniGPT. GPT From Scratch in PyTorch

MiniGPT is a GPT-style language model that I built from scratch in PyTorch following the ideas taught in Andrej Karpathys GPT-from-scratch lecture.

## Overview

MiniGPT builds a decoder-only Transformer language model from scratch and trains it on a character-level text dataset.

MiniGPT aims to understand how GPT-style language models work inside by building the parts with PyTorch.

## What I Built

- MiniGPT built a character-level tokenizer.

- MiniGPT split the data into training and validation sets.

- MiniGPT created a -batch data loader.

- MiniGPT added token embeddings.

- MiniGPT added positional embeddings.

- MiniGPT implemented causal self-attention.

- MiniGPT implemented multi-head self-attention.

- MiniGPT added a feed-forward network.

- MiniGPT added residual connections.

- MiniGPT added layer normalization.

- MiniGPT stacked multiple Transformer blocks.

- MiniGPT implemented autoregressive text generation.

- MiniGPT evaluated training and validation loss.

## Model Configuration

- MiniGPT set the context length to 256.

- MiniGPT set the embedding dimension to 384.

- MiniGPT set the number of attention heads to 6.

- MiniGPT set the number of Transformer layers to 6.

- MiniGPT used a dropout rate of 0.2.

- MiniGPT used the AdamW optimizer.

## Dataset

MiniGPT trains a model on the Shakespeare dataset.

MiniGPT learns to predict the character based on the previous characters, in a sequence.

## Architecture

```text

Input Text

↓

Character Tokenization

↓

Token Embeddings + Positional Embeddings

↓

Transformer Blocks

├── Causal Self-Attention

├── Multi-Head Attention

├── Feed-Forward Network

├── Residual Connections

└── Layer Normalization

↓

Language Model Head

↓

Next-Token Probabilities

↓

Generated Text

```
