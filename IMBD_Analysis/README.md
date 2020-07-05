IMDB Dataset
=
This is a built-in dataset in the tensorflow_dataset library with the name <i>imdb_reviews</i>.

The dataset contains 50,000 (25,000 train and 25,000 test) real-world reviews given by people all various movies in english language. In the dataset these reviews are classified as negative(0) or positive(1).

Link :  https://www.tensorflow.org/datasets/catalog/imdb_reviews

So the challenge here was to build a NLP classifier which learn features related to a negative and a positive review depending on the reviews in the dataset. The basic idea is to use 
embedding i.e. grouping together word with similar meaning. The classifier would then learn which words corresponds to a positive and negative review. All the words present in the whole dataset
were tokenized i.e. given a numerical value since Deep Learning works only on numbers. These words together corresponds to a corpus or a dictionary for that particular model.

Whenever a new unseen review is given to the model to classify, it will first tokenize the review using the tokenizer instance used during the training and then it will compare the features 
learned from the training based on the corpus and embedding and then depending on the meaning
it understood, it will then classsify the review as positive or negative.

The model isn't prefect and does not any prior experience with language, so it might give wrong prediction on a extermely simple sentence.

