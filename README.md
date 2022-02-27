# Little-Search-Engine
Rutgers CS112: Assignment 3

This project implements a simple search engine for text documents using hash tables.

## Description

This application serves as a little search engine in which a user enters keywords they wish to search for in a pool of documents and is provided with a list of relevant documents which contain matches to these keywords.

The application takes in a docs.txt file which contains a list of documents serving as the information pool to search through, and a noisewords.txt file which stores words that are commonplace (such as "the") to be ignored by the search engine. The search engine creates two hashtables, one which indexes all keywords from all input documents, and another which stores all noise words. Each key word is mapped to a list of occurences ordered based on it's frequency in a document using binary search. The output of a user's search is a list of the 5 most relevant documents based on the frequency of searched keywords. 

The search engine is implemented to do two main things: (a) gather and index keywords that appear in a set of plain text documents, and (b) search for user-input keywords against the index and return a list of matching documents in which these keywords occur.

### Executing Program

To execute this program: a driver can take as inputs a file that contians the names of all the documents (such as docs.txt) and then set up a LittleSearchEngine object to call its methods as needed to test the implementation. The docs.txt and noisewords.txt filenames will be sent in as arguments to the makeIndex method in LittleSearchEngine.
Some example textfiles are provided: ptest1.txt, ptest2.txt, ptest1opp.txt


All use of this code must comply with the [Rutgers University Code of Student Conduct](http://eden.rutgers.edu/%7Epmj34/media/AcademicIntegrity.pdf).
