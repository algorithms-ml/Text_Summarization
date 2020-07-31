# Text-Summarization
 This repo contains text summarization use cases

Abstractive Text Summarization:

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


Extractive Text Summarization :

Approaches for Abstractive Text Summarization:
1.	Pretrained models such as BERT, GPT-2, XLNet etc. We can apply these through 'bert-extractive-summarizer'
2.	Fine tuning of transformer based architecture. However, these would requird good comupational infrastucture
3.	Unsupervised Approaches (TextRank)

I have tried out the 3rd approach which consists of a graph based reprentation of documents and then applyying TextRank algo to find the important sentences


Steps followed:
1. Read data into Python and Data cleansing steps
2. Select a story for further steps (in step 1.3 of the code)
3. Apply TF-IDF reprentation
4. Apply Graph reprentation
5. Apply TextRank Algorithm
6. Define a threshold
7. Select top n sentences (based on importance) and create summary

Note:
1. The code is not highly automated. We need to manually run the prograam step by step. It requires manually selecting the story (in section 1.3 of the code) for further processing
2. Then run remaining portion of the code to get the summary

System Requirement/Dependencies:
1. Python 3.7
2. NLTK
3. networkx




