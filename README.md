# Twitter Sentiment Analysis

Sentiment analysis (or opinion mining) is a natural language processing (NLP) technique used to determine whether data is positive, negative or neutral.

<p align="center">
<img  src="https://github.com/vj-vanshika/TwitterSentimentAnalysis/blob/main/static/t2.jpg" class="center">
</p>

## Applications :

Twitter sentiment analysis allows you to keep track of what's being said about your product or service on social media, and can help you detect angry customers or negative mentions before they escalate.

## What exactly i've done?

I have created a Web Application for sentiment analysis using TextBlob and flask framework.
The interface allows you to type a keyword and get the sentiment analysis with a general report and visual representation of analysis.

## Steps:
1. Fetched real time tweets from Tweepy API, encoded them into utf-8 and saved them into a csv file called result.csv 
2. Nextly, i have cleaned tweets using regular expressions.
3. The cleaned version of data is then provided to Textblob model to obtain the polarity.
4. The polarity is categorized into 7 types namely:
        <br>    1.POSITIVE (0.3<polarity<=0.6) </br>
        <br>    2.WEAKLY POSITIVE (0<polarity<=0.3) </br>
        <br>    3.STRONGLY POSITIVE (0.6<polarity<=1)</br>
        <br>    4.NEGATIVE (-0.3<polarity<=-0.6)</br>
        <br>    5.WEAKLY NEGATIVE (-0.3<polarity<0)</br>
        <br>    6.STRONGLY NEGATIVE (-0.6<polarity<=-1)</br>
       <br>     7.NEUTRAL (polarity=0)</br>
5. According to the polarity obtained, a pie chart is constructed using matplotlib and saved in plot1.png    and updated with every keyword search.
6. All of the web templates and python code is connected via using Flask.

For more details you can go through with my project report uploaded as TwitterSentiment.pdf
