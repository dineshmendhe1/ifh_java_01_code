# IFH Seminar 01
# Sentiment-Analysis-in-Java
A sentiment analysis code that tells us the sentiment of a sentence based on a dictionary of words which tag words as negative and positive and give them a score from -10 to 10


Overview:
    The main idea of the project is to calculate the TweetScore for a tweet. To perform the analysis we use a .csv file of tweets
    The words, taken one at a time are checked if they are present in the Stopwords. If the word is present
    in the list of Stopwords, the word is ignored and the code moves on to the next word. If a word is not present in the Stopwords' list, it 
    is checked for in the AFINN library which has been converted into a hasmap with <word, score> as key value pair. The score of the word is 
    fetched and added to the TweetScore, which is the overall score for a tweet. The TweetScore is addition of scores of all the individual 
    words present in the AFINN library. If a word is not present in the AFINN library, it is skipped.


Resource References:
  -AFINN dictionary (Contains the the score based on the extremity of the word)
          Link: http://www2.imm.dtu.dk/pubdb/views/publication_details.php?id=6010
  -Stopwords: Words which don't have any sentiments, such as I, We, You etc.

