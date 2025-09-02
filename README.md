Python Practice Problems

This repository contains three short Python exercises I worked on for practice. Each problem focuses on a simple but important Python concept: sorting strings, replacing words with emoticons, and unpacking list elements.  

1.  Alphabet Soup Problem
Code:
   def alphabet_soup(word):
    return ''.join(sorted(word))
    
This function takes a word and rearranges its letters in alphabetical order.  
It’s a simple way to practice string manipulation.

2. Code:
def emotify(sentence):
    emoticons = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": ">:("
    }
    words = sentence.split()
    result = []
    
    for word in words:
        if word.lower() in emoticons:
            result.append(emoticons[word.lower()])
        else:
            result.append(word)
   return " ".join(result)
   This one replaces certain words in a sentence with their corresponding emoticons.
   
3. Code: 
    def unpack_list(lst):
    first, *middle, last = lst
    print("first:", first)
    print("middle:", middle)
    print("last:", last)

  This function unpacks a list into three parts:
 the first element
 everything in the middle
 the last element
