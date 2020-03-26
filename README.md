# Emojifier
Thisproject aims at developing a model which inputs a sentence and finds the most appropriate emoji to be used with this sentence to make the text messages more expressive.

![](https://github.com/parasgulati8/Emojifier/blob/master/images/Capture.JPG)

There are two versions of the Emojifier. First version uses the averaged values of all word vectors in a sentence and then using softmax function for classification.
![](https://github.com/parasgulati8/Emojifier/blob/master/images/emojifierv1.png)

Second method uses the LSTM layers to learn the long range dependencies in the text and thus performs better than the first model.
![](https://github.com/parasgulati8/Emojifier/blob/master/images/emojifier-v2.png)
## Word Vector Representations

We use pretrained 50-dimensional GloVe embeddings to represent words in vector form in a 50 dimensional space. The word embeddings were taken from Stanford open source project : https://nlp.stanford.edu/projects/glove/.

## Conclusion

- Emojifier is an application that inputs a sentence and (such as "Let's go see the baseball game tonight!") and finds the most appropriate emoji to be used with this sentence (⚾️). 
- It uses GloVe representation to turn words into 50-dimensional vectors which are then input to the model for training and prediction.
- Pretrained GloVe embeddings are used and the weights were not changed while training the LSTM model.
- The LSTM model achieves an accuracy of 82% on test set

## References
The project is a part of an online course on Sequence Models that I completed on Coursera

https://www.coursera.org/learn/nlp-sequence-models
