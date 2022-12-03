# Natural_language_processing

## Long Short Term Memory (LSTM network) 
- an artificial neural network that is an advanced version of recurrent neural network (RNN), was designed to model the chronological sequences of data.

This is a simple project to recognize the tweet emotions with the use of machine learning through natural language processing that is used for text and speech data (unstructured data)

#### Tokenizing
The very first part of speech data is to convert the text into tokens.
Tokenizing by word and tokenizing by sentence are the types used to manage the data that helps in working with smaller data pieces of text that are still coherent in nature and have a meaningful context with the rest of the text.
For this project I have used tokenizing by word to help identify the particular words in the sentence that has emotional meaning attached to it and the algorithm tries to find words that often conveys emotions.

#### Truncating and Padding

As the text data is unstructured it would not be accepted everytime by the model that expects the same data length for every entry in the data. Hence the long and short tweets has to be tkaen care of before feeding them into to model for the training.
- Truncating
-This is used to limit the size of the tweeets that are longer than than the acceptable tweets which in this case is 50 words per tweet.
- Padding
-As the word suggest this method has been used to pad the shorter tweets under the required lenght with zeros. This means that the padding is done after the original tweets till the length of 50 

#### MODEL
The model consists of embedding and LSTM layers.
*The embedding layers* maps the inputs to vectors of integers that can be used by the model for training. As the vocabulary of the dataset is finite, we would have a finite set of integers representing the words
*Bi-directional LSTM layer* helps in feeding the sequence information in both directions- backwards and forwards to learn and preserve the future and past information.

Below figure demonstrates a basic structure of a single LSTM cell.
![LSTM cell](https://user-images.githubusercontent.com/84092636/205437703-cab105ca-8859-4970-814f-1211b85a5bfa.jpeg)
