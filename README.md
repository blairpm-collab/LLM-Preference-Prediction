# LLM Preference Prediction using Chatbot Arena

This repository contains the code and analysis for my Honours dissertation: *Fine-tuning Large Language Models to Predict Human Preference using Chatbot Arena Conversations*.

## Project Overview
This project evaluates the effectiveness of zero-shot prompting (Condition A) compared to Quantized Low-Rank Adaptation (QLoRA) fine-tuning (Condition B) for predicting human preferences. The experiments were conducted using the `microsoft/Phi-3.5-mini-instruct` model. 

Due to hardware constraints on the available Tesla T4 GPU (14.5 GB VRAM), the training dataset was reduced to 2,000 examples to prevent OutOfMemory errors, which is detailed in the project's Deviations Log.

## Repository Files
* **`LLM_Preference_Prediction_Code.ipynb`**: The main Google Colab notebook containing data preprocessing, QLoRA configuration, model training, and evaluation scripts.
* **`requirements.txt`**: The list of Python dependencies and versions required to run the notebook.

## Key Results
* **Condition A (Zero-Shot Prompting):** Accuracy = 0.3915
* **Condition B (QLoRA Fine-Tuning):** Accuracy = 0.3785
