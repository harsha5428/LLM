Climate Sentiment 

Project Overview : 
This project involves fine-tuning a BERT-based transformer model for sentiment analysis on climate-related text data. The model is trained to classify text data into different sentiment categories (e.g., positive, neutral, negative) and analyze the impact of climate change discussions on social media and other platforms.

Dataset
The dataset used for this project is sourced from the Hugging Face Datasets library, specifically the "Climate Fever" dataset. This dataset contains text data related to climate change, including claims and corresponding labels.

Training Dataset Size: 1300
Test Dataset Size: 400

Model
The model used in this project is based on the BERT (Bidirectional Encoder Representations from Transformers) architecture. BERT is a pre-trained language model that can be fine-tuned for various NLP tasks, including sentiment analysis.

Base Model: bert-base-uncased
Fine-Tuned for: Sentiment classification on climate-related text data

Training Procedure
The model was fine-tuned using the following training arguments:

Evaluation Strategy: Evaluation at the end of every epoch
Batch Size (Train): 8
Batch Size (Eval): 8
learning-rate : 2e-5
Number of Epochs: 5
Weight Decay: 0.01
The training was conducted on a GPU-enabled environment to accelerate the fine-tuning process.

Assign3_final.ipynb: Jupyter Notebook used to Contains the ClimateSentimentAnalysis class, which handles data loading, model training, evaluation, and sentiment prediction.,fine-tune the BERT model and evaluate its performance on the validation set.
results/: Directory to store the output results, including the trained model and evaluation metrics.

Results
The fine-tuned model achieves the following results:

Accuracy: 0.96
F1 Score: 0.97

Edge Cases and Considerations
Edge Cases: The model may struggle with ambiguous or sarcastic statements, which can be challenging for sentiment analysis models.

Acknowledgments
Special thanks to Hugging Face for providing the transformer models and datasets.
