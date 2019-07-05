# Natural Language Processing

The use of natural language processing has exploded over the last decade. Appilcations that require machines to understand natural human speech patterns are abundant and substantial improvements in these systems has increased their utility. Within the educational space NLP is used to interpret human speech for the prupose of understanding human problems and recently an online tutor passed a limited version of the [Turing Test](https://en.wikipedia.org/wiki/Turing_test) when it was [indistinguishable from teaching assistants in a college class](http://www.news.gatech.edu/2017/01/09/jill-watson-round-three).

## Project Objective:

The purpose of this project is to process a set of documents, run a sentiment analysis of these documents and then generate topic models of those documents by applying Latent Dirichlet Allocation (LDA) topic modelling to a set of documents. The documents consist of student notes that the graduate-level Core Methods in Data Mining course. 

## Datasets:
  
  * week-list.csv
  * class-notes (containing CSV files with student notes)
  * negative-words.txt
  * positive-words.txt

## Procedure:

First, the document files in the class-notes file were binded together into a dataframe. Then, the student notes were cleaned and processed with tm package. A word cloud was generated, which is shown below.

![wordcloud](https://github.com/lizarova777/Natural_Language_Processing_Project/blob/master/Word_Cloud.png)

Then, the dataframe with students' notes was merged with the week-list, and a sentiment analysis was performed. In particular, a visualization with the sum of the sentiment score over weeks was generated, which is shown below.

![sentimentanalysis](https://github.com/lizarova777/Natural_Language_Processing_Project/blob/master/Change_of_the_Sentiment_Score_Over_Time.png)

LDA Topic Modelling was performed on the documents in order to generate topics. A visualization was created displaying a sentiment for each week and one important topic for that week, which can be seen below.

![maintask](https://github.com/lizarova777/Natural_Language_Processing_Project/blob/master/An_Important_Topic_and_Sentiment_Per_Week.png)


  
  