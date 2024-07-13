# Bert-Extractive-Text-Summarizer
A bert model is a deep learning architecture based on a multi-head attention 
mechanism that weights the importance of each part of the input data 
differently. It follows an encoder-decoder structure but does not rely on 
recurrence and convolutions in order to generate an output. Transformers are 
designed to process sequential input data.


Process 
-• BERT Embeddings: The input text is tokenized and passed through a 
pre-trained BERT model to obtain contextual embeddings for each 
word/token in the text. These embeddings capture the semantic 
meaning and context of each word within the sentence. 
-• Sentence Embeddings: The contextual embeddings obtained from 
BERT are aggregated to represent each sentence in the input text. 
Various aggregation methods can be used, such as averaging or 
pooling the embeddings of individual tokens within the sentence. 
-• Clustering with K-Means: The sentence embeddings are then 
clustered using the K-Means algorithm. K-Means partitions the 
sentence embeddings into K clusters based on their similarity, where 
K is the desired number of sentences in the summary. 
-• Sentence Selection: Once the clusters are formed, the centroid of 
each cluster is computed. The sentences closest to each centroid are 
selected as representatives of their respective clusters and included in 
the summary. 
-• Summary Generation: The selected sentences from each cluster are 
concatenated to form the final summary.
