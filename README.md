# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Open the file in read mode and read it using the read() function.
### Step 2: 
Using for loop to iterate throught the texts in the file.
### Step 3: 
Split the text using space separator. We assume that words in a sentence are separated by a space character.
### Step 4:  
Check if the text is present or not in the dictionary created.
### Step 5: 
If no, word count equals to 1.
### Step 6: 
If yes, word count increments by 1 and the dictionary is printed
## PROGRAM:
```python

import sys
fp=open(sys.argv[1],"r")
d={}
for i in fp:
    for w in i.split():
        if w not in d.keys():
            d[w]=1
        else:
            d[w]+=1
print(d)
```
### OUTPUT:
![cmdl](https://user-images.githubusercontent.com/98278161/214896829-4dc8f3f8-c32a-4591-bc0a-b049a44bd049.jpeg)


## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
