# Impact of Data on Image Captioning Models

This project investigates how **dataset quantity** and **quality** affect the performance of **image captioning models**.  
The experiment involves **fine-tuning a pre-trained Git-based model** on the *One Piece* image caption dataset using the 🤗 **Transformers** library.

---

## Key Objectives

1. **Fine-tune** a pre-trained vision-language model on an image captioning dataset.  
2. **Evaluate** model performance using **Word Error Rate (WER)**.  
3. Analyze the **impact of dataset size** (quantity) and **filtered captions** (quality) on caption generation.

---

## Part 1: Fine-Tuning the Image Captioning Model

- Dataset: [`YaYaB/onepiece-blip-captions`](https://huggingface.co/datasets/YaYaB/onepiece-blip-captions)  
- Base Model: `microsoft/git-base`  
- Evaluation Metric: **WER (Word Error Rate)**  

### Training Highlights:
- 90% training / 10% testing split  
- Model trained for 50 epochs  
- Uses Hugging Face `Trainer` for training and evaluation  

### Example Outputs:
The model generates captions for anime-style images.  
Evaluation is based on how closely the generated captions match the true captions.

---

## Part 2: Impact of Dataset Quantity

- Trained model on a **subset of 400 examples**.  
- Compared generated captions to those from the full dataset.  
- Observed performance degradation due to reduced data exposure.

---

## Part 3: Impact of Dataset Quality

- Filtered out training samples containing specific words: `"man"`, `"shirt"`, `"tie"`.  
- Retrained the model and compared results with the unfiltered dataset.  
- Analyzed the model’s descriptive accuracy after quality reduction.

---

**## Hello and Welcome

Thank you for visiting my GitHub page!  
I’m currently in the process of uploading my previous projects and doing my best to make them publicly available in an organized and clear manner.  

At the moment, I’m adding each project with some **light updates and clarifying adjustments**, and I plan to include more **comprehensive notes, explanations, and detailed READMEs** very soon — to help others better understand each project’s idea and usage.  

If you have any questions, suggestions, or would simply like to connect, I’d be delighted to hear from you:  
- [LinkedIn](https://www.linkedin.com/in/wajdalrabiah)  
- [X (Twitter)](https://x.com/wajdalrabiah)  

Thank you again for your time and interest.  
Your feedback and interaction are always appreciated

> _More updates coming soon — stay tuned!_  **
