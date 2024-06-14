# ADReSS-challenge---Alzheimer-s-disease-prediction-using-spontaneous-speech

Using the dataset provided for ADReSS challenge for interspeech 2020, i experimented with the classification problem. 
Specifically: 
1) I only use the transcripts and not the audio files
2) I only work on the predicion of AD, (0-1 binary classification) although with some minor changes i believe the code will be useful for predicting the MMSE score as well

The repository is seperated in 3 folders. Each folder contains the file that created a certain dataset, and another file with the different classification models and their classification metrics (f1 score, accuracy, recall, precision): 
1) Characteristics dataset: Refers to the dataset that was created using different characteristics from the speech of each participant and from CHAT encoding. The folder contains the file that created the dataset and also a file with different classification models, using grid search and many graphs. This repository is my thesis and the graphs were used for showing my results, that is why there are so many, though i believe they are probably useful 😁
2) BERT dataset: The dataset i used for BERT, and also BERT used in transfer learning
3) Combined dataset: Basically the characteristics dataset combined with sklearn's CountVectorizer. This particular combination could be adjusted to the characteristics dataset, but i wanted to see the differences in the results when i used the CountVectorizer and when i didn't so i seperated them.

Results: There are many different results, but the best model acheived the following scores for the test set: 
f1 score:  0.9165217391304347
accuracy:  0.9166666666666666
precision: 0.9195804195804196
recall:  0.9166666666666666
