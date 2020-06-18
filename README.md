# Verify-OnlineForumAnswers
### *Verifying the credibility of answers on online health forums using text classification methods*

Online forums have made life so much simpler for all of us. The convenience of getting your questions answered by anyone around the globe in a matter of minutes is what makes it a success. For us programmers, stack overflow is a holy shrine - it always surprises me to find a post where someone has also gone through a very specific issue or error that I have gone through and in most cases, these queries are answered.
But along with convenience comes another problem - the credibility of the source. Sure, most forums have credibility assigned to the user based on how many people have found his/her answers useful in the past, number of answers, days of activity etc. The problem we explore here is on the health forums. Similar ways of evaluating credibility are also there but how do we know who's a doctor and who's not?

## Problem 
Are answers posted by an acutal doctor or not?

We tackle this by comparing the posts made by doctors with other professionals. There are some text charecteristics that we, as humans, can identify to evaluate whether a person is a doctor or not - the vocabulary. This is precisely what we compare

## Hypothesis 
Doctors have a distinctive use of language, like the frequency with which they use medical terms, that can identify them through their text

So let's now explore this method further and see if we can execute this idea to classify answers as one made by doctors and one made by other professionals

## Dataset
1500 answers by doctors and 1500 answers by other professionals

## Approach

1. Combine the two datasets into one
2. Define a custom tokenizer
3. Use the custom tokenizer along with SpacY to preprocess the text documents into a corpus
4. Vectorize the corpus into a TF-IDF vector
5. Train a Naive Bayes Classifier on this data
6. Evaluate results
