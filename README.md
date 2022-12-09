# Arabic-Full-Name-Verification-NLP-Model

Arabic Full Name Verification It is a NLP Model that takes a person full name depend on the Arabian structure and verify if this name is a person real name or fake one using Natural language processing (NLP)

# Data Generation: 
- Used the dataset <a href="https://github.com/abdallah-elsawy/Arabic-Full-Name-Verification-NLP-Model-/blob/main/Names%20web%20dataset/Arabic_names.csv">Arabic_names.csv</a> which contains Arabian real name from both gender to generate the real data.
- The same dataset used to generate our fake names part.
- combine both real & fake data to one file to be our dataset.

# Core model:

- 1- Classical ML approach: using some classical machine learning like *MultinomialNB*, *LogisticRegression*, *SGDClassifier* as classification model.
- 2- Deep Learning Approach: using PyTorch to build deep learning model by finetuning an *Arabic-BERT* model trained on ~8.2 billion words then use our labeld dataset to train and test the model.

# Deployment:

- The deployment done using *Flask*. I used Flask to get the user input from the HTML page, then send the response to tested it on the saved model weights. And the predicttion of the name verification is sent to back to HTML page to show it. like in the following gif.


<img src="https://github.com/abdallah-elsawy/Arabic-Full-Name-Verification-NLP-Model-/blob/main/Deployment%20Usin%20Flask/deploy.gif" alt="Deployment gif" width="75%">


# Next Step

- Build the model using Tensor-Flow.
- Deploy on Flutter App & Docker
