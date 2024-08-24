# Spam Detection Project

In this project, I aim to build a model for detecting spam messages. I have tried three different approaches to tackle this problem:

1. **Simple Naive Bayes Approach**: This was the first approach I tried. Naive Bayes is a simple and fast algorithm, often used as a baseline in text classification problems. I used the `CountVectorizer` and `TfidfTransformer` from `sklearn` to convert the text data into numerical features that the Naive Bayes model could use. The advantage of this approach is its speed - both in terms of training and testing. However, it may not always provide the best performance, especially for complex text data.
2. **SMOTE Naive Bayes Approach**: In the second approach, I used the Synthetic Minority Over-sampling Technique (SMOTE) to balance out the data. This was done to check if balancing the data would make the model less biased and improve its performance. The same Naive Bayes model was used after the SMOTE process.
3. **Local Language Model Approach**: In the final approach, I used a local language model (DistilBert) for spam detection. This approach is often considered one of the best for text classification problems, as it can capture the context of the text data better than traditional methods. I chose DistilBert because it provides a good balance between performance and computational resources. However, it's worth noting that DistilBert can take some time to train depending on the computational resources available.

Each of these approaches has its own strengths and weaknesses. Naive Bayes is much faster to train and test, making it a good choice for initial exploratory analysis or when computational resources are limited. On the other hand, DistilBert, while requiring more computational resources and time, often provides better performance and is a very good combination of implementation effort, training time, and results.

## How to Run the Notebook

To run the notebook, you will need to download the dataset from [this link](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset?resource=download) and place it inside a folder called `data` in the root directory of the project.

The project structure should look like this:

├── data
│ └── spam.csv
├── notebooks
│ └── spam_detection.ipynb
└── [README.md](http://readme.md/)