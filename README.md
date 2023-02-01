# Articles-Classification

The objective is to classify the type of news articles. Is a Multi-class classification problem with the following classes: Opinion, Reporting and Satire.
For thi aim, a DistilBert Transformer was implemented and fine-tuned, making additional tests in the process like:
  - Changing the 512 tokens to send to the transformer: First 512, Last 512, and some part of the beggining and some of the end.
  - Making an extractive summary of the article to reduce the tokens and avoid loosing important information to classify the article.
  - Extracting the embedding of the input from the last layer of BERT corresponding to the [CLS] (an embedding that is aware of the context of each token) and combining it with NLP characteristics of the text as input to different ml algorithms like SVM, MLP and Random Forest.
  - Modifying the BERT structure by adding an MLP to enable the combination of categorical and numerical features for the final classification.
  - Using SHAP for explainability, to understand why the model is predicting some classes and see if it is possible to improve the performances.

In this repository we can see different notebooks that try to show some of the code used to make this tests.
