# Personally Identifiable Information (PII) Detection in Educational Data

This project focuses on **automated PII detection** in educational datasets using **natural language processing (NLP)** techniques to ensure privacy while enabling the creation of high-quality, public datasets for research.

## Table of Contents
- [Project Overview](#project-overview)
- [Techniques Used](#techniques-used)
- [Models Evaluated](#models-evaluated)
- [Results and Performance](#results-and-performance)
- [Future Scope](#future-scope)
- [Market Opportunities](#market-opportunities)

## Project Overview
This project was developed as part of the **Data Mining Principles Final Project** in collaboration with **Vanderbilt University** and **The Learning Agency Lab's Kaggle Competition**. We aim to automate the detection and cleansing of **personally identifiable information (PII)** such as student names and sensitive details in educational datasets. This ensures that the datasets can be publicly shared without compromising privacy.

**Motivation**: PII in educational data restricts the availability of high-quality public datasets. Manual detection is costly and unscalable. Our goal is to revolutionize this process by automating PII detection using NLP techniques, particularly **Named Entity Recognition (NER)** models.

## Methodology
- **Named Entity Recognition (NER)**: We used **Bidirectional Encoder Representations from Transformers (BERT)** to detect PII, with a focus on identifying and classifying named entities like people, locations, and organizations.
- **Data Augmentation**: Created additional samples to complement the provided Kaggle dataset using various **Large Language Models (LLMs)**.
- **Exploratory Data Analysis**: Included visualizations like word clouds to understand the frequency of PII in the dataset. PII such as "student names" constituted 49% of all labels, with no significant correlation between document length and the presence of PII.

## Models Evaluated
### 1. **DistilBERT**
   - A more compact version of BERT, optimized for efficiency.
   - **70% Accuracy** with a smaller architecture, **40% smaller** and **60% faster** compared to BERT.
   - Suitable for large-scale processing of text data.
   
### 2. **LUKE (Language Understanding with Knowledge-based Embeddings)**
   - Integrates external knowledge sources to enhance entity recognition.
   - **95% Accuracy**, with more granular results, especially for specific industries like **education** and **healthcare**.

## Future Scope
Our long-term vision includes expanding the application of our PII detection solution to other sectors:
- **Healthcare**: Detect and redact sensitive patient data, ensuring compliance with regulations like HIPAA.
- **Legal**: Use PII detection for automated redaction of sensitive legal documents, protecting client confidentiality.

## Deployment
The solution is designed for **scalable deployment** using **Google Cloud Platform** (GCP) to handle large datasets and provide real-time PII detection.
