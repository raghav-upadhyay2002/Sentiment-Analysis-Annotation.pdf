# Sentiment Analysis Annotation

This project focuses on sentiment analysis of customer reviews for refurbished mobile phones from Amazon. The goal is to classify reviews as positive or negative using a manually annotated dataset and a neural network model.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Future Work](#future-work)

## Introduction
Sentiment analysis helps businesses understand customer feedback and make data-driven decisions. This project uses a balanced dataset of Amazon reviews, annotated by two annotators, to train and evaluate a neural network model for binary sentiment classification.

## Dataset
- **Source:** Reviews were manually collected from the Amazon review section of a refurbished phone seller.
- **Annotations:**
  - Annotator 1: Primary annotations with balanced sentiments.
  - Annotator 2: Independent review to introduce variability.
  - Golden Label: Final consensus label after resolving disagreements.
- **Distribution:**
  - Positive: 50.5%
  - Negative: 49.5%

## Methodology
1. **Annotation Guidelines:**
   - Positive: Reviews expressing satisfaction or delight.
   - Negative: Reviews expressing dissatisfaction or frustration.
2. **Data Preprocessing:**
   - Text cleaning, tokenization, stopword removal, and TF-IDF vectorization.
3. **Visualization:**
   - Pie charts showing sentiment distributions for Annotators and the Golden Label.
   - Agreement and disagreement rates between annotators.

## Model Training and Evaluation
- **Model Architecture:**
  - Built using TensorFlow's Sequential API with dense and dropout layers.
  - Optimized with binary cross-entropy loss and the Adam optimizer.
- **Metrics:**
  - Accuracy: 80%
  - F1 Score: 0.80
  - Cohen's Kappa: 0.91
- **Visualization:**
  - Loss and accuracy trends over epochs for training and validation datasets.

## Results
- High agreement rate (94%) between annotators.
- Balanced dataset with robust classification performance.
- Visualizations highlighted sentiment distribution and inter-annotator reliability.

## Technologies Used
- Python (TensorFlow, Scikit-learn, Matplotlib, Pandas, Numpy)
- LaTeX for report generation

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sentiment-analysis-annotation.git
   cd sentiment-analysis-annotation

2.	Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.	Run the preprocessing and training script:
    ```bash
    python main.py
    ```
4.	Visualize results:
	•	Check the output plots and evaluation metrics generated during training.

## Future Work

	•	Expand the dataset to include more nuanced sentiments like neutral or mixed.
	•	Experiment with advanced NLP techniques like transformers for better classification accuracy.
	•	Implement active learning to refine annotations dynamically.

## References

	•	Amazon Reviews Dataset
	•	Scikit-learn Documentation: Cohen’s Kappa
	•	Grammarly for grammar checks and rephrasing.
## Author
    Raghav Upadhyay
    Feel free to contribute or suggest improvements for this project!    

