# language-transformers-BERT

The code examples are from my medium article, "How to apply BERT and similar language models to customer text processing", https://medium.com/@kai.chaza_92389/how-to-apply-bert-and-similar-language-models-to-customer-text-processing-27189433cce.

In the article I walk through several examples of sentence transformers using the famous BERT model. The repo has got both BERT and distilBERT examples, as well as Tensorflow and Pytorch examples. All the code was tested on a Google colab notebook, but if you want environment specific requirements. I also give the requirements.txt file to replicate my local environment, where I run the code on a GPU. 

The examples can still work without a GPU, but I highly recommend running the fine-tuning model training examples on a machine with a GPU or at least in Google Collaboratory as there are 67,000 sentences in the training set, and they all need to be vectorized and tokenized, and then a gradient descent optimization process needes to run over 3 epochs, which could take several hours without a GPU. 

BERT should take about 30 min to train on a GPU if running on Google Colab. The size of the file also gets quite large when training BERT, so a GPU with less than 8 GB of memory will most likely fail.
