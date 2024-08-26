# PA1---Introduction-to-Python-Programming
"This repository contains Python code that solves programming problems titled: *Alphabet Soup*, *Emoticon*, and *Unpacking List*."

Below is a preview of the code, but there is also a Jupyter notebook uploaded in the files section.

## 1. Alphabet Soup Problem
``` python
def alphabet_soup (word):
    #Sort the characters and join them into a single string
    return ''.join(sorted(word))

#Ask the user for input
user_word = input("Enter a word: ")

#Get and print the alphabetically sorted word
print(alphabet_soup(user_word))
```

## 2. Emoticon Problem
``` python
def emotify(sentence):
    #Dictionary with words and their emoticons
    emoticon_dict = { "smile": ":)", "grin": ":D", "sad": ":((", "mad": ">:("}

    #Split the sentence into a list of words
    words = sentence.split()

    #Replace words with emoticons if they are in the dictionary
    for i in range(len(words)):
        if words[i] in emoticon_dict:
            words[i] = emoticon_dict[words[i]]

    #Combine the list of words back into a single string
    new_sentence = " ".join(words)

    #Return the sentence with emoticons
    return new_sentence

#Ask the user for a sentence
user_sentence = input ("Enter a sentence: ")

#Print the sentence with emoticons
print(emotify(user_sentence))
```

## 3. Unpacking List Problem
``` python
#Ask the user for input
user_input = input("Enter a list of numbers separated by spaces: ")

#Convert the user input into a list of integers
writeyourcodehere = list(map(int, user_input.split()))

#Unpack the list
#'first' gets the first element
#'*middle' gets all the elements between the first and last
#'last' gets the last element
first, *middle, last = writeyourcodehere

#Print the variables
print("first:", first)
print("middle:", middle)
print("last:", last)
```
