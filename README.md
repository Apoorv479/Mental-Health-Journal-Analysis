# Mental Health Journal Analysis System

An AI-powered Mental Health Journal Analysis System that analyzes user journal entries to identify emotions, detect stress triggers, generate summaries, and provide personalized mental wellness guidance.

The project combines Transformer-based Natural Language Processing (NLP), emotion classification, keyword extraction, trigger analysis, and guidance generation to help users gain deeper insights into their emotional well-being.

---

## Project Overview

Mental health journaling is widely used for self-reflection and emotional expression. However, traditional journaling applications provide limited analytical capabilities.

This project transforms raw journal entries into meaningful emotional insights through:

- Emotion Detection
- Keyword Extraction
- Trigger Identification
- Mood Classification
- Summary Generation
- Personalized Guidance Generation
- Weekly Emotional Trend Analysis

---

## AI Pipeline

User Journal Entry
↓
Emotion Detection (DistilRoBERTa)
↓
Keyword Extraction (KeyBERT)
↓
Trigger Detection
↓
Mood Classification
↓
Summary Generation
↓
Personalized Guidance
↓
Weekly Insights

---

## Repository Structure

### 1. Mental_Health_Emotion_final_Model.ipynb

This notebook contains the complete Emotion Detection Model Training Pipeline.

#### Major Components

- GoEmotions Dataset Loading
- Data Cleaning and Preprocessing
- Tokenization
- Label Encoding
- DistilRoBERTa Fine-Tuning
- Model Evaluation
- Model Saving
- Model Backup

#### Model Details

- Base Model: DistilRoBERTa
- Dataset: GoEmotions
- Emotion Classes: 28
- Classification Type: Multi-Label Classification
- Epochs: 3
- Learning Rate: 2e-5
- Batch Size: 16
- Optimizer: AdamW

#### Output

A fine-tuned emotion classification model capable of identifying multiple emotions from journal entries.

---

### 2. Journal_analyzer.ipynb

This notebook contains the complete Journal Analysis Application Pipeline.

#### Features

##### Emotion Detection

Uses the fine-tuned DistilRoBERTa model to detect emotional states from journal entries.

##### Keyword Extraction

Extracts meaningful keywords using KeyBERT.

##### Trigger Detection

Identifies potential emotional triggers such as:

- Academic Stress
- Work Stress
- Financial Stress
- Relationship Issues
- Health Anxiety

##### Mood Classification

Classifies overall mood into:

- Positive
- Neutral
- Negative

##### Summary Generation

Generates a concise emotional summary based on detected emotions and triggers.

##### Personalized Guidance

Provides supportive recommendations based on emotional analysis.

##### Weekly Analysis

Generates:

- Weekly emotional trends
- Dominant emotions
- Common triggers
- Weekly guidance

---

## Technologies Used

### Artificial Intelligence

- DistilRoBERTa
- Transformers
- KeyBERT
- PyTorch
- Hugging Face

### NLP

- Emotion Classification
- Keyword Extraction
- Text Analysis
- Multi-Label Classification

### Backend

- Python
- FastAPI

### Development Environment

- Google Colab
- Jupyter Notebook

---

## Dataset

### GoEmotions Dataset

The emotion detection model is trained using the GoEmotions dataset developed by Google Research.

#### Dataset Statistics

- 58,000+ text samples
- 27 emotions + Neutral
- Human-annotated labels

### Examples of supported emotions:

 - admiration,
   amusement,
anger,
annoyance, approval,
caring,
confusion,
 curiosity,
   desire,
disappointment,
 disapproval,
 disgust,
 embarrassment,
excitement,
fear,
 gratitude,
grief,
 joy,
 love,
 nervousness,
optimism,
 pride,
 realization,
 relief,
 remorse,
 sadness,
 surprise,
 neutral
---


## Future Improvements

- Context-Aware Trigger Detection
- Advanced Recommendation Models
- Retrieval-Augmented Generation (RAG)
- Multi-Language Support
- Real-Time Emotional Monitoring
- Conversational Mental Wellness Assistant

---

## Disclaimer

This project is intended for educational and research purposes only.

The generated insights and guidance should not be considered a substitute for professional mental health advice, diagnosis, or treatment.

---

## Author

Final Year Project

AI-Powered Mental Health Journal Analysis System
