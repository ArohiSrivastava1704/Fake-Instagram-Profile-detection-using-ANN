# Fake-Instagram-Profile-detection-using-ANN

Overview
This project focuses on detecting fake Instagram profiles using Artificial Neural Networks (ANN). The goal is to classify Instagram profiles as real or fake based on various features extracted from user data. The system uses supervised learning techniques to create a predictive model that helps in identifying fraudulent accounts.

Project Objectives
Understand the patterns of fake and real Instagram profiles.
Extract relevant features from profile data for effective classification.
Build an Artificial Neural Network (ANN) model for detection.
Evaluate and optimize the model for high accuracy and reliability.
Dataset
Source: [Mention if publicly available or self-collected]
Size: [Specify the number of rows and columns]
Features:
Quantitative: Number of followers, following, posts, likes, comments, etc.
Qualitative: Profile bio details, account verification status, profile picture.
Behavioral: Frequency of posts, engagement rates, and account age.
Target Variable: Fake/Real (binary classification: 1 = Fake, 0 = Real)
Technologies Used
Programming Language: Python
Libraries:
Data Manipulation: pandas, numpy
Visualization: matplotlib, seaborn
Machine Learning: scikit-learn, tensorflow, keras
Text Analysis (if required): nltk, spacy
Project Workflow
Data Collection:

Gather data from Instagram profiles using APIs or web scraping.
Ensure compliance with Instagram's terms of service.
Data Preprocessing:

Clean the dataset by handling missing values and outliers.
Encode categorical features (e.g., bio status, verification status).
Scale numeric features for ANN compatibility.
Feature Engineering:

Extract new features like engagement ratio, post-to-follower ratio, etc.
Perform text analysis on bios (e.g., keyword presence, sentiment).
Model Development:

Design an ANN architecture with:
Input layer (based on the number of features).
Hidden layers (fully connected, with ReLU activation).
Output layer (single neuron with sigmoid activation for binary classification).
Compile the model with:
Loss function: binary_crossentropy.
Optimizer: Adam.
Metric: accuracy.
Model Training and Evaluation:

Split the data into training and testing sets (e.g., 80-20 split).
Train the ANN on the training set with appropriate epochs and batch size.
Evaluate on the testing set using accuracy, precision, recall, F1-score, and ROC-AUC.
Results and Insights:

Analyze the model’s performance and identify key indicators of fake profiles.
Visualize important metrics, like loss and accuracy curves.
Deployment (Optional):

Create a web or mobile interface where users can input profile details to check for authenticity.

Results
Accuracy: [96%]
Other Metrics:
Precision
Recall
F1-Score
ROC-AUC
Key Findings:
Accounts with high follower-following ratios and frequent engagement are often genuine.
Profiles with generic bios and disproportionate engagement ratios are more likely to be fake.
Challenges and Future Work
Challenges:
Limited availability of labeled data for fake profiles.
Balancing the dataset for genuine vs. fake accounts.
Future Work:
Incorporate advanced NLP techniques for bio and comment analysis.
Explore other machine learning models for better accuracy.
Deploy the solution as a real-time Instagram fake profile detection tool.
