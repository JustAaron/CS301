# CS301-101 Project Proposal

# What is the problem that you will be investigating? Why is it interesting?
On the social media website Twitter, users can publicly post “tweets” that consist of text and possibly images or tags. In the unfortunate event of a real-world disaster, some affected users may post tweets that describe the event in real-time. Tweets can be unclear and not all tweets that involve certain “disaster-related” keywords are describing a disaster. The problem we will be investigating is identifying whether a given tweet is describing a legitimate disaster or not. This topic is interesting as it involves Natural Language Processing (NLP). 

# What reading will you examine to provide context and background?
We will be reading the Kaggle challenge that inspired the topic, along with any guides that it includes. We will also likely find more generalized articles on Natural Language Processing and use those as well. 

# What data will you use? If you are collecting new data, how will you do it?
We will be using the data provided by the Kaggle challenge. This dataset consists of 10,000 tweets as well as their labels. Tweets consist of a unique id, text of the tweet, keyword (may be blank), and location (may be blank). The labels are either 1 (for a real disaster) or 0 (not a real disaster). 

# What method or algorithm are you proposing? If there are existing implementations, will you use them and how? How do you plan to improve or modify such implementations? You don’t have to have an exact answer at this point, but you should have a general sense of how you will approach the problem you are working on.
We know that this is a classification problem because the labels are discrete values of 1 or 0. We may choose to view the text as a “bag of words”, meaning that the words themselves each have meaning, but the order does not change their individual meaning. We may also choose to use word2vec, which does consider the order of words, to produce word embeddings. 

# How will you evaluate your results? Qualitatively, what kind of results do you expect (e.g. plots or figures)? Quantitatively, what kind of analysis will you use to evaluate and/or compare your results (e.g. what performance metrics or statistical tests)?
At a minimum, we expect to compare the success of the results using just the proportion of correctly labeled instances vs the proportion of incorrectly labeled instances. Using the ROC curve, We will aim to maximize the True Positive Rate while minimizing the False Negative Rate. 
