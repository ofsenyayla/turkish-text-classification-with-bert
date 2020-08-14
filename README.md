# **Turkish Text Classification with BERT**

The purpose of this notebook to make a text classifier for the Turkish language by using BERT.  
  
BERT is a transfer learning that is used in NLP. It is based on Transformer architecture. It consists of combining more than one encoder. It processes words from left to right and right to left simultaneously, so it is faster than Bi-LSTM's.
  
I used bert-based-uncased model and tokenizer in this notebook.
  
In this notebook, I used the TTC-3600 dataset. It is a dataset that contains 3600 Turkish news from 6 different topics (600 each). [The dataset can be accessed here.](https://github.com/denopas/TTC-3600 "TTC-3600 Dataset")

The data was in separate folders according to the news category and every news was in separate .txt files. So, first I concatenated each news in a pandas data frame and added a new column named 'section' that is the category of the news. Then, I stemmed each sentence with the Zemberek library. Finally, I cleared stopwords, punctuations, and numbers and saved the final dataset as 'df_clean.csv'. The notebook does not contain these steps.

I wrote this notebook on Google Colab, so I could use a GPU.
