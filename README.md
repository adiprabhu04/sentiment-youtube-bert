# Uncovering Audience Insights: YouTube Comment Sentiment & Persona Analysis

## 🚀 Project Overview

This project implements an end-to-end Natural Language Processing (NLP) pipeline to analyze YouTube video comments. The primary goal is to perform fine-grained sentiment analysis and identify distinct audience personas based on their expressed sentiment and semantic content. This provides valuable insights for understanding audience reactions and for effective audience segmentation.

The project goes beyond basic sentiment classification to reveal *who* is engaging with content and *how* they feel.

## ✨ What This Project Achieved

* **Comprehensive Data Pipeline**: Successfully developed and implemented a full pipeline for YouTube comment analysis, from data acquisition to insightful interpretation.
* **Robust Data Preparation**: Achieved clean and high-quality textual data through a rigorous preprocessing phase that handles noise, ensures language consistency (English), and filters for meaningful content.
* **Advanced Sentiment Classification**: Successfully fine-tuned **DeBERTa-v3-small**, a state-of-the-art transformer model, for multi-class sentiment classification, demonstrating the ability to leverage powerful pre-trained models and address data challenges like class imbalance with weighted loss.
* **Meaningful Audience Segmentation**: Effectively identified and segmented the YouTube audience into distinct personas (e.g., "Critic," "Casual Viewer," "Superfan") by applying **K-Means clustering** to rich feature vectors derived from DeBERTa embeddings and weighted sentiment scores.
* **Actionable Insights through Visualization**: Generated clear, interactive visualizations using Plotly to represent the discovered audience personas and their associated sentiment distributions, enabling intuitive understanding of audience characteristics.
* **Practical Application**: Built a system capable of performing real-time sentiment prediction and persona assignment for new, unseen comments, showcasing immediate utility for content analysis.

## 🛠️ Technologies & Skills

* **Programming Language**: Python
* **NLP**: `nltk`, `langdetect`, `emoji`, `transformers` (Hugging Face)
* **Machine Learning**: `scikit-learn` (Clustering, Model Evaluation)
* **Deep Learning**: PyTorch (for DeBERTa model operations)
* **Data Handling**: `pandas`, `numpy`
* **Visualization**: `plotly`
* **Performance**: `concurrent.futures` (Multithreading for efficient data processing)


## 🛣️ Future Directions

This project lays a strong foundation for advanced audience understanding. Here are some ideas for future expansion:

* **Integrate with a Web App**: Deploy the sentiment and persona models into a user-friendly web application (e.g., Streamlit, Flask, FastAPI) for live analysis of YouTube channels or specific videos.
* **Dynamic Clustering**: Explore techniques to dynamically determine the optimal number of clusters rather than fixing it to 3.
* **Time-Series Analysis**: Analyze how sentiment and persona distributions evolve over time, identifying trends or responses to specific content.
* **Explainable AI (XAI)**: Implement tools like SHAP or LIME to understand *why* a specific comment is classified with a certain sentiment or assigned to a particular persona.
* **Multi-Platform Analysis**: Extend the scraping capabilities to other social media platforms (e.g., X/Twitter, Reddit) to gather a more comprehensive view of public opinion.
