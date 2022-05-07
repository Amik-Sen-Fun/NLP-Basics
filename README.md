# NLP-Basics

Contains Notes and Codes realted to DataCamp NLP course.
Let's Start with our First Course: 

# Introduction to Natural Language Processing in Python

## Introduction to regular expressions

- WHat is Natural Language Processing?
  - It is a field of study focusing on making sense of language using statistics and computers.

## What is Regular Expressions?
- It is a string with a special syntax which is used to match patterns in another string.
- regex is implemented in python as :
  ```python
  import re
  re.match('abc','abcdef') # Here 'abc' is matched with 'abcdef'
  # It is also possible to match pattern based on certain understanding.
  re.match('\w+','Hi! there') # \w+ is used to match words 
  ```
  Some similar regex syntaxes are:
  
|pattern|matches|example|
|---|---|---|
|\w+|word|'Magic'|
|\d|digit|9|
|\s|space|' '|
|\S|No space|''|
|+ or \*|greedy match|'aaaaaa'|
|.\*|wildcard|'username87'|
|\[a-z\]|lowercase group|'abcdef'| 

In python regex is implemented using `re`. Some important functions of which are:

- `re`: the module
- `split`: splits the given string
- `findall`: finds all occurences of the pattern in the string
- `search`: search for a pattern
- `match`: match an entire string or substring based on a pattern

The output of these can be regulated and found as objects or iterators etc.

## Introduction to Tokenization

It is the process of converting a string or documents into smaller chunks known as tokens. There are certain rules for tokenising the words.

The python library `nltk` is used for it.

Why tokenise?
- Easier mapping of parts of speech
- Matching Common Words
- Removing unwanted tokens


## Advanced Tokenization

|pattern|matches|example|
|---|---|---|
|\||OR|`\d\|\w` macthes words or digit|
|A-Za-z+|Upper and Lower alphabets|'ABCdef'|
|0-9|Numbers|9|
|A-Za-a\-\.|Upper case and lower case and - and .|google-in.com|
|(a-z)|a,- and z|a-z|
|(\s+|,)|spaces and comma|' ,'|

## Word counts with bag-of-words

Bag of words is a basic method for finding topics in a text.
The steps include:
- Tokenize the words
- Count the frequency of each token
- More the frequency, more central it is to the meaning of the sentence.

For better input it is important to preprocess the text.  
Some preprocessing are:
- Tokenization
- Lowering Case
- Lemmatization/Stemming
- Removing Stop words, punctuations and unwanted tokens



Moving to our second course

# Feature Engineering for NLP in Python
