# Basic Sentiment Analysis using Hive

To determine each tweet's score and identify whether the tweet had a positive, negative, or neutral sentiment, I created an excel file calls tweet.csv with 20 tweets. The file includes some columns such as postid, twitter_handle, content, num_comments, num_retweets, likes. Then, I put tweet.csv and Dictionary.txt into Hive. I kept getting some null values when I load the excel file into Hive. After trying to figure out what I did wrong several times, I realized that some tweets with line breaks had some null values. Cleaning data in excel is necessary. Next, to split up each tweet into words, I created the table split_ntl0039. Next, I joined two tables that included dictionary information and split words to get the score of every word of tweets. Finally, I grouped the scores by postid and twitter_handle to get each tweet's score and determined whether the tweet had a positive, negative, or neutral sentiment based on the scores. I kept getting some null values when I load the excel file into Hive.   

To improve the Sentiment Analysis using Hive, the dictionary file needs more words and develops in specific fields based on analysts' purpose. Some tweets did not show the scores because the words on those tweets do not match the dictionary file words. This lacking of words leads to an incomplete analysis of the tweets.   

![Optional Text](https://user-images.githubusercontent.com/86505407/146411090-340e0e24-cb2a-4e8a-a7d9-940661498654.png)

![Optional Text](https://user-images.githubusercontent.com/86505407/146411514-7b82c7d0-bd3f-4a10-80e8-9038ffd74142.png

![Optional Text](https://user-images.githubusercontent.com/86505407/146411148-4f163603-327a-48b9-8fac-383935b2e35f.png)

![Optional Text](https://user-images.githubusercontent.com/86505407/146411165-5c0b5037-788d-4ee8-9cac-02735312a00d.png)

![Optional Text](https://user-images.githubusercontent.com/86505407/146411175-873d042f-6d20-443b-9c02-b32a401cc8a9.png)


