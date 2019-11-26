Introduction to Language Model and its Applications
===================================================

Language Model: **A model of the probability of a sequence of words**

A language model can assign probability to each possible next word. And also, help in assigning a probability to an entire sentence. 

Applications:
_____________
* Predicting upcoming words or estimating probability of a phrase or sentence is useful in noisy, ambiguous text data sources 
* Speech Recognition: E.g.: P('recognize speech') >> P('wreck a nice beach')
* Spelling Correction: E.g.: P('I have a gub') << P('I have a gun')
* Machine Translation: E.g.: P('strong winds') > P('large winds')
* Optical Character Recognition/ Handwriting Recognition
* Autoreply Suggestions
* Text Classification (discussed with python implementation of a simple N-gram model)
* Text Generation (discussed this with Char-level and Word-level language models)
