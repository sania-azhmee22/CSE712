
# CSE712
Master’s project on Explainable Detection of Online Sexism using NLP. Applied preprocessing, tokenization, SMOTE, and BiLSTM (TensorFlow/Keras) for binary classification, achieving 81.43% validation accuracy. Fine-tuned BERT (PyTorch, Hugging Face) with TF-IDF for 4-class sexism detection, achieving ~69% accuracy and ~0.70 F1 score.
As part of my Master’s project, I worked on Explainable Detection of Online Sexism, which focused on detecting sexist language from online text and classifying different forms of sexism. The project included two separate tasks.

In Task A, I worked on a binary classification problem to identify whether a post was sexist or non-sexist. The dataset was preprocessed through text cleaning, tokenization, label encoding, and sequence padding. I used an existing Bidirectional LSTM-based model with TensorFlow and Keras for training and evaluation. To reduce the impact of class imbalance, I applied SMOTE oversampling and class weighting techniques. The model achieved around 81.43% validation accuracy in the initial training phase, while another run produced 79.21% validation accuracy with an F1 score of 0.7939.

In Task B, I classified sexist posts into four categories: threats, derogation, animosity, and prejudiced discussion. For this task, I used TF-IDF vectorization and fine-tuned a pre-trained BERT (bert-base-uncased) model using PyTorch and Hugging Face Transformers. The final model achieved approximately 69% overall accuracy with weighted and macro F1 scores close to 0.70. The project involved working with NLP preprocessing, sequence classification, model evaluation metrics, and transformer-based text classification methods in Python.

Sexism is a form of discrimination based on a person’s gender or sex. Sexism can lead to violence and creates an oppressive environment that prevents most women from fully participating in public life. Creating a model that is able to identify sexist texts could lead to several positive outcomes for society. Such a model could be used to prevent and counter sexist language in different situations, such as in public and private communications, media, and social networks. This could help promote gender equality and create a more inclusive and respectful environment.

<img width="960" height="540" alt="edos_vectors" src="https://github.com/user-attachments/assets/c03aba8b-6ba2-4a90-a1ed-805bd0b131f8" />

In our project we focused solely on identifying signs of sexism and classifying them. In particular we complited 3 different tasks:

Task A - Binary Sexism Detection: a two-class (or binary) classification where systems have to predict whether a post is sexist or not sexist.
Task B - Category of Sexism: for posts which are sexist, a four-class classification where systems have to predict one of four categories: (1) threats, (2) derogation, (3) animosity, (4) prejudiced discussion.
