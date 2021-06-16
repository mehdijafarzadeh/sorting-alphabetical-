## Moby Dick Challenge
Count the number of words in the full text of Moby Dick!
How many times does the word whale appear?
What are the top ten most used words?
Save the dictionary of word frequencies as a json file
Bonus: Create a line plot of the ordered word frequencies.
Clean the text, store each unique word as a key in a dictionary and the corresponding word frequency as its value. The resulting data structure should look like this:

{
    'the': 827,
    'python': 34,
    ...
}    
Hints
These functions might be useful to look at:

- open('myfile')
- txt = "hallo"
- txt.replace()
- txt.split()
- file.read()
- json.dump()

### More Hints

Read in the ./data/mobydick.txt textfile as a single string (use the f.read() function of the file connection object f). Store the string in a variable with the name txt.
Convert everything to lowercase.
Remove the line breaks \n (Hint: Use the txt.replace(old, new) function to replace substrings in txt with ' '). Are there any other characters that you could clean from the text?
Split the cleaned text using whitespace as separator (look at the txt.split() function). You get a list of single words.
Create an empty dictionary. Loop over the list of words:
Check if the word is already in the dictionary.
If yes, increase the counter for this word by 1.
If no, add it as key to the dictionary and assign it the value 0.
