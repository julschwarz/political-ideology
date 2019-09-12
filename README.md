# DETECTING POLITICAL IDEOLOGY IN YOUTUBE COMMENTS USING MACHINE LEARNING

## Keywords
Political ideology detection, text classification, machine learning, SVM, YouTube


## ABSTRACT
Political ideologies are diverse and complex but can be approximated through one's choice of words. In this project we used three different approaches to predict political ideology in YouTube comment data. The first SVM model was trained on 500 self-labeled YouTube comments, the second one on 36.000 presidential candidate’s Twitter post and the last one on 4000 sentences of US parties’ electoral manifestos. Challenges were the access to training data, different content and syntax of available training data sources, class imbalances in the data as well as manual labeling. We found that when a political tendency classifier is trained and tested on data in the same corpus, accuracy is higher, indicating that data from one source can hardly be generalized to another one. Nevertheless, if no similar training data is available, data from different sources that match the time, topic and syntax can yield reasonable results. Ambiguous and low polarized comments have been excluded when dropping the initially labeled neutral class. To handle class imbalances, we propose two solutions: a weighted SVM, increasing the loss for wrongly predicted democratic comments, and an SVM trained on a balanced data set. Finally, we created a political ideology classifier that can yield up to 79% accuracy on the task of classifying YouTube comments.

## Data Sources:
### 1. YouTube comments scraped from political news channels (MSNBC & Fox News) 
A set of 500 YouTube comments on the topic of the Mueller report and Russia investigation was scraped using YouTube's API and then manually labeled.

### 2. Tweets of presidential candidates 2020
We scraped 35.924 tweets published between May 25 and June 24 from presidential candidates and labeled them according to the party of the author.

### 3. Party manifestos dataset
One classifier was trained on parties’ electoral manifestos from 2016, that are made publicly available by
the Manifesto Project. This train set consists of 3.882 sentences covering a large range of political topics dating back 2016. It's available on https://manifesto-project.wzb.eu. 
