# POS Tagger
### By:Sabah Ibrahim ###

## Description:

What is POS tagging and why is it important and helpful?

<p> POS tagging or part of speech tagging is used to classify words by their part of speech based on the definition of the word and its context. 
This is extremely useful in natural language processing as it can help categorize words and build parse trees and can help in named entity recognition and sentiment analysis. A great example of this application in real life, is the app Grammarly, which is able to tell how your writing may sound to your readers. 
<hr --------------------------------------- />  
The main problem is that manually annotating words with POS tags is time consuming and super tiring. As we are trying to train computers to be able to understand and speak our language, it is very logical to first train computer to be able to accurately POS tag words in a dataset. </p>
<hr --------------------------------------- />     
How exactly do we do that?
Human languages are extremely complex, whereas computers are more systematic, how can we train computers to tag differently in different contexts?
How to we train a tagger that based on meaning of words and thier frequency/influence in its context?
<hr --------------------------------------- />  
This program tries to answer some of these questions and I will also be talking about some improvements that can be made. There are different methods that can be used and will be helpful based on the kind of dataset we are dealing with and what we wnat to achieve from it. 
    This program uses two classifiers: Naive Bayes and Decision tree and POS tags using two different representations: label encoder and one hot encoder. 
From my findings it seems that one hot encoder worked best, as it seems to take care of columns where there maybe no data existent and keeps that from messing up the data representation. 
<hr --------------------------------------- /> 
<p>Given more time these are some ways I would like to extend this code:</p>

<p> One way I would like to try and classify data is using the bag of words representation data. Bag of representation is really good for this data set and the way it works is that it calculates the frequency of unique words in the data set. This is a good way to represent data that we can weigh words based on their occurrence and repentance in the dataset. This does not preserve word order, or meaning of words, but rather best tells which words are most frequent and tags them accordingly. This may not be the best representations if we are trying to look beyond frequencies of words, but this dataset was open ended and not meant to be analyzed for some particular reason, hence this method would work well. The method is slightly more complex, and may require more time for training and testing.</p> 
<p> In addition to that, I would like to try the tf-id vector, had I had more time to work on it. I tried implementing the tf-id vector, but consistently kept getting extremely low values for precision, accuracy, and recall. The tf-id does take longer to train and test compared to the other methods. The reason why tf-id may work well, is because it us able to deal with the problems that bag of words representation have. It allows for words that are more meaningful, and more frequent to have more influence than words, that are rare, bag of words representation can weigh some words unintentionally more. This also preserves the sentence structure, so this would be a great representation.</p>

## Give a short description on how to run your code

This code is pretty easy to run. The variable df holds the directory address for the data and this can be changed to reflect the address of the data you would like to POS tag. The output will show how well the methods performed.
