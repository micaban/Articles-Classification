# Articles-Classification
In this repository, you will find some notebooks showcasing the fine-tuning and testing of a DistilBert Transformer for the classification of news articles into three classes: Opinion, Reporting, and Satire. The project involves several experiments to improve classification performance and gain insights into the model's decision-making process.
Here are the main experiments and techniques explored:

1) Token Selection: Different strategies were tested to choose the tokens to send to the DistilBert Transformer, including using the first 512 tokens, the last 512 tokens, and a combination of tokens from the beginning and end of the article.

2) Extractive Summarization: To reduce the number of tokens and retain essential information, extractive summarization techniques were applied to the articles.

3) Feature Engineering: The embeddings from the last layer of the DistilBert model corresponding to the [CLS] token, which captures context information, were combined with additional NLP characteristics of the text as input to various machine learning algorithms like SVM, MLP, and Random Forest.

4) Modified BERT Structure: The BERT architecture was modified by adding an MLP (Multi-Layer Perceptron) to enable the combination of both categorical and numerical features for the final classification.

5) SHAP for Explainability: SHAP (SHapley Additive exPlanations) was utilized to gain insights into the model's predictions and understand why certain classes were predicted, potentially leading to performance improvements.

The notebooks that try to show some of the code used to make this tests.

The final model was uploaded to the SemEval2023 competition and achieved the 6th position with a F1-score of 58.6%. The paper that describes the model and methodology is [Unisa at SemEval-2023 Task 3: A SHAP-based method for Propaganda Detection](https://aclanthology.org/2023.semeval-1.122/) presented in ACL 2023
