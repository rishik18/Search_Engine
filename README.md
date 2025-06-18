# Search_Engine

## Introduction
This project implements a search engine using a compressed Trie and an Inverted index.
The code is written in Python using a Jupyter Notebook.

## Implementation
1) Input files: The HTML files are saved locally. Six Wikipedia pages related to bears have
been used.
2) Reading the files: The files are read in using BeautifulSoup. The text for each webpage
is stored in a dictionary using the web pages as keys.
3) Tokenization: The data is tokenized using regex.
4) Filtering: The stopwords are filtered using the stopword corpus from the NLTK library.
5) Creation of inverted index: The inverted index is implemented using a dictionary where
words are keys and the values are the webpages they occur in along with the number of
times the word appears in the page.
6) Creation of the Compressed Trie:
+ Trie nodes: Each node contains a dictionary of child nodes and a boolean
representing whether the child is the end of the word.
+ Compressed trie methods: <br>
i) Init: initializes the root node. <br>
ii) Longest_common_prefix: finds and returns the longest common prefix
given two strings. <br>
iii) Print_trie: prints out the contents of the tree. <br>
iv) Insert: For inserting items into the tree. <br>
v) Search: searches for a word in the trie and returns True if the word is
present in the Trie, otherwise, it returns False. <br>
7) Search and ranking:
+ Search: <br>
i) Each word in the input string is searched in the trie.<br>
ii) If found in the Trie, the word is searched in the inverted index.<br>
iii) The inverted index provides the occurrence list and number of
appearances.<br>
+ Ranking:<br>
i) The pages are sorted by the number of appearances and printed out.<br>
ii) If there are more than multiple words then the intersection of the sets of
pages is printed out.<br>
iii) If the word is not present in the trie then a message that the word is not in the
vocabulary is printed out.<br>

## Sample outputs

### Sample 1
![image](https://github.com/user-attachments/assets/7a324966-f5b7-4cff-acdd-cf0cf0a7e004)

### Sample 2
![image](https://github.com/user-attachments/assets/2a57dba8-9f30-4b70-ae8b-70b8a12c6068)

### Sample 3
![image](https://github.com/user-attachments/assets/86113234-0519-44d1-ab68-1bc8a27454e7)

### Sample 4
![image](https://github.com/user-attachments/assets/cbd332d6-ed59-40d1-a125-ff9da03d7fe0)




