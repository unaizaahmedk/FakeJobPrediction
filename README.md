# Fake Job Post Prediction

This project aims to detect fraudulent job postings using machine learning and deep learning techniques. We used the [**Employment Scam Aegean Dataset (EMSCAD)**](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction), which contains around 18,000 job postings labeled as real or fake. The work is inspired by and based on methodologies proposed in two research papers on job scam detection using NLP and neural networks.

We implemented and compared three main approaches:

- A Sequential Neural Network (SNN) using GloVe embeddings
- A set of Traditional Machine Learning classifiers
- A Deep Neural Network (DNN) trained with SMOTE and Stratified K-Fold Cross-Validation to handle class imbalance

## Results

### Sequential Neural Network (GloVe Embeddings)
- Test Loss: 0.0546  
- Accuracy: 98.43% 
- AUC Score: 99.72%

### Traditional Machine Learning Models

| Model                         | Accuracy | Precision | Recall  | F1 Score |
|------------------------------|----------|-----------|---------|----------|
| K-Nearest Neighbors (KNN)    | 95.25%   | 94.50%    | 95.25%  | 93.38%   |
| Random Forest                | 95.05%   | 93.42%    | 95.05%  | 93.33%   |
| Support Vector Machine (SVM) | 94.94%   | 90.13%    | 94.94%  | 92.47%   |
| Decision Tree                | 94.94%   | 93.10%    | 94.94%  | 93.30%   |
| Naive Bayes                  | 92.31%   | 90.87%    | 92.31%  | 91.56%   |
| Multilayer Perceptron (MLP)  | 95.11%   | 95.35%    | 95.11%  | 92.88%   |

### Deep Neural Network (DNN) with SMOTE & Stratified K-Fold
- Average Accuracy: 77.38%
- Average Precision: 15.61%
- Average Recall: 83.25%

Although the DNN had lower overall accuracy, it achieved significantly higher recall, making it the most effective model for identifying fraudulent job posts, which is often the top priority in such applications. 

## Contributors

- [@Khoula Adil](https://github.com/KhoulaAdil)
- [@Uroosha Zehra Abidi](https://github.com/Uroosha4048)
