# mlops-assignment-2
This model is a fine-tuned version of distilbert-base-cased for Goodreads book review genre classification. The model was trained using the Hugging Face Transformers library on the UCSD Goodreads dataset as part of an MLOps assignment.

The objective of the project was to build a complete MLOps workflow including:

fine-tuning a Hugging Face model
experiment tracking using Weights & Biases (W&B)
training on Kaggle GPU
deployment to Hugging Face Hub
Model Details
Base Model: distilbert-base-cased
Task: Text Classification
Number of Labels: 8
Framework: Hugging Face Transformers
Training Platform: Kaggle GPU
Experiment Tracking: Weights & Biases (W&B)
Labels
The model predicts the following genres:

children
comics_graphic
fantasy_paranormal
history_biography
mystery_thriller_crime
poetry
romance
young_adult
Training Details
Dataset
UCSD Goodreads Reviews Dataset

Training Hyperparameters
Epochs: 5
Batch Size: 16
Learning Rate: 3e-5
Max Sequence Length: 512
Evaluation Metrics

Metric	Score
Accuracy	0.58437
F1 Score	0.58095
Eval Loss	1.16838
Usage
from transformers import pipeline

classifier = pipeline(
    "text-classification",
    model="YOUR_USERNAME/distilbert-goodreads-genres"
)

result = classifier("This book was amazing and full of adventure.")
print(result)

Project Links
GitHub Repository: https://github.com/g25ait2143-spec/mlops-assignment-2
Kaggle Notebook: https://www.kaggle.com/code/palaganisaichaitanya/notebook97772a1f61
Weights & Biases Dashboard: https://wandb.ai/g25ait2143-iitj/mlops-assignment2/runs/a6gt5pfq?nw=nwuserg25ait2143

Author
Name: Palagani Sai Chaitnya
Course: MLOps | PGD AI Program | IIT Jodhpur
