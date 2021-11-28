# CS301-101 Project Proposal, Aaron Lee

# What is the problem that you will be investigating? Why is it interesting? 
A common use case for search engines such as Google is to receive answers to questions. These questions will often be given in the form of natural language. The problem is that computers do not read information in the same way as humans do, and so the goal is to transform the question into one that a machine would be able to understand. Natural Language Processing (NLP) is interesting as it can be used for use cases such as a Q&A search system. A Q&A system can be more complicated than some other forms of NLP problems because natural language must be processed for both the question and the answer. The sentiment of the question must be translated to know what the topic of interest is. The sentiment of any articles that are related to this topic must also be translated.

# What reading will you examine to provide context and background? 
We will be reading the documentation behind Haystack, a state-of-the-art long-form Q&A API, along with any of the guides or tutorials that it includes. We will also likely find more generalized articles on Natural Language Processing and use those as well. 

# What data will you use? If you are collecting new data, how will you do it? 
We will be using the Stanford Question Answering Dataset (SQuAD) to train the Haystack pipeline. This dataset consists of over 100,000 question-answer pairs sourced from Wikipedia. These question-answer pairs are produced by humans through crowdsourcing and so are more diverse than other QA datasets. 

# What method or algorithm are you proposing? If there are existing implementations, will you use them and how? How do you plan to improve or modify such implementations? You don’t have to have an exact answer at this point, but you should have a general sense of how you will approach the problem you are working on. 
We will be using the existing Haystack implementation but modified such that the “knowledge base” is more generalized. With this generalized knowledge base, we hope to be able to answer more generalized questions. 

# How will you evaluate your results? Qualitatively, what kind of results do you expect (e.g. plots or figures)? Quantitatively, what kind of analysis will you use to evaluate and/or compare your results (e.g. what performance metrics or statistical tests)?
At a minimum, we expect to compare the success of the results using just the proportion of correctly labeled instances vs the proportion of incorrectly labeled instances. Using the ROC curve, We will aim to maximize the True Positive Rate while minimizing the False Negative Rate.
