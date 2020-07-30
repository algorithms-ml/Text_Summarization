# Text-Summarization
 This repo contains text summarization use cases


Approaches for Abstractive Text Summarization:
1.	Seq2Seq model with Bidirectional LSTM and attention mechanism
2.	Transformer based architecture(e.g - Google's BERT, Mocrosoft's UniLM etc.)

I have tried out the first approach which consists of a architecure based on Seq2Seq model with Bidirectional LSTM and attention mechanism

Steps followed:
1. Read data into Python and Data cleansing steps
2. Saves the clened model in a pickle format for further usage
3. Data Preparation for training which consists of tokenizing the stories and summaries (highlights)
4. Apply GLoVe pretraied embedding
5. Built custom layer for attention
6. Build model acthitecure for training
7. Build inferencing logic
8. Model training 
9. Model prediction logic (here using the actual summary to get the prediction - can be updated to give prediction based on test set)


Notes:
The code is in a working condition. 
However, I could not tune the hyperparameters not I could train it for more epochs to get better accuracy result.
If GPU is available we can retrain the model.

 
Due to system constraint I have used only stories that have sequence lenth   <= 1200. This comes around 577 article.

Due to system constraint cound not tune the hyeperparamers

Due to system constraint could not play around with the model atchitecture

I have not implemented model evaluation metrics (ROUGE) as of now.



System Requirement/Dependencies:
1. TF 2.2.x
2. Python 3.7
3. GloVe






