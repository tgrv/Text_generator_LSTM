# Text Generation using LSTM

This is a small fun project to demonstrate the use of LSTMs in learning text sequences, and thereafter generating new word sequences.

For this activity, we will use a text corpus consisting of Shakespeare's sonnets, which is available at the following link:
https://ocw.mit.edu/ans7870/6/6.006/s08/lecturenotes/files/t8.shakespeare.txt

The sonnets are just a subset of the entire available corpus. We will train our LSTM based model to learn from these sonnets, and generate poetry of our own! 

Steps performed:

1. Download corpus from given link.
2. Tokenize corpus.
3. Create n_gram sequences for each line in corpus.
4. Pad sequences keeping maximum length of each sequence equal to that of the longest sentence.
5. Create predictors and labels for these sequences, i.e. for each n_gram tuple, its label should be the next occuring word.
6. Create LSTM based model. The advantage of using bidirectional LSTMs is that it keeps information about previously occuring words as well.
7. Run the model, and plot the training accuracy and loss in real time along-with each epoch.
8. After the model has trained, we will predict next `n` words by giving an initial seed text.  