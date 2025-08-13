# Embeddings-for-CLIP

This repository was created as part of the **Vision Language Models (VLMs) Bootcamp** conducted by **OpenCV University**.

## 📌 Overview

Text and image embeddings are vectors of numbers (e.g., a 512×1 vector) learned by a model that capture the gist of a sentence or a picture.

Instead of raw pixels or words, each point in the vector encodes a bit of meaning — so two text strings that “feel” similar in meaning end up with vectors close together, and the same goes for visually similar images.

**CLIP** (Contrastive Language–Image Pretraining), developed by OpenAI, enables us to create embeddings for text strings and images in a **shared embedding space**. For example, the vector for an image of a cat and the vector for the text “a cat” will be close together compared to “an airplane”.

## 🎯 Goals

In this notebook, we use CLIP to:

1. Obtain embeddings for text strings.  
2. Compare embeddings of different text strings.  
3. Obtain embeddings for images.  
4. Compare embeddings of different images.  
5. Compare embeddings of images and text strings.

## 🛠 Model Used

We use the CLIP Vision Transformer variant `openai/clip-vit-base-patch32` from HuggingFace

## 🔍 How It Works
1. Tokenization: Text strings are converted into tokens (numerical representations of words) and padded with start and end tokens.
2. Embedding Generation: The CLIP model returns a 512-length embedding for every text string or image.
3. Similarity Measurement: Embeddings are compared using cosine similarity to find semantic closeness



