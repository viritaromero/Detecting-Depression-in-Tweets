# Detecting-Depression-in-Tweets
Detecting Depression in Tweets using Baye's Theorem

Depression is a mental illness that is not taken seriously in some countries. I grew up in Mexico and I never got exposure to mental illness education at school or at home. As a kid, I felt sad sometimes and I knew about people getting sad because of difficult times, and even getting depressed but I never thought about people looking for professional help to overcome depression. Some people have been diagnosed with depression and don’t take medication to overcome it. They just continue their lives without medication and getting worse.

There are many experiences that can cause us depression, such losing a loved one, losing a job, getting a divorce and other tough situations can lead a person to feel blue, lonely and overwhelmed. It’s normal to get these feelings when we feel stressed. Everybody have experimented sadness at times. However, depression is very different from this. Depression is a psychiatric disorder that need to be addressed with medication.
Definition of Depression

According to Our World in Data Website, Depressive disorders occur with varying severity. The WHO’s International Classification of Diseases (ICD-10) define this set of disorders ranging from mild to moderate to severe. The The Institute for Health Metrics and Evaluation( IHME) adopt such definitions by disaggregating to mild, persistent depression (dysthymia) and major depressive disorder (severe).

All forms of depressive disorder experience some of the following symptoms:

    (a) reduced concentration and attention
    (b) reduced self-esteem and self-confidence
    (c) ideas of guilt and unworthiness (even in a mild type of episode)
    (d) bleak and pessimistic views of the future
    (e) ideas or acts of self-harm or suicide
    (f) disturbed sleep
    (g) diminished appetite

Worldwide Statistics

    322 million people worldwide live with depression.

Depression is the leading cause of disability worldwide. Almost 75% of people with mental disorders remain untreated in developing countries with almost 1 million people taking their lives each year. In addition, according to the World Health Organization (WHO), 1 in 13 globally suffers from anxiety. The WHO reports that anxiety disorders are the most common mental disorders worldwide with specific phobia, major depressive disorder and social phobia being the most common anxiety disorders.
Depression on Social Media

Social media platforms are becoming an integral part of people’s life. They reflect user’s personal life. People likes to share happiness, joy and sadness on social media. These platforms are used for researchers to identify the causes of depression and detect it.

I was reading an old article in the Time News Website about how Twitter knows when you’re depressed and the possibility of creating an artificial intelligence model that can scan your Twitter feed and tell you if you’re at risk for depression or receive notices from third parties, for instance, that warned you that you may want to seek help, just based on an automated scan of your tweets. I guess, that day has finally come. There are many ways for detecting sentiment in tweets.

Detecting earlier depression can be a huge step to address the mental illness and offer support to the people suffering from this terrible mental illness.
Creating a model to detect depression in tweets

In Machine Learning, there are many ways for sentiment analysis such: decision-based systems, Bayesian classifiers, support vector machine, neural networks and sample-based methods.

After reading some papers about using different Machine Learning and artificial intelligence techniques to detect depression on Social Media, I decided to apply sentiment analysis through a powerful theorem from probability theory called Baye’s Theorem. The model will be write in python and it will tell whether a given tweet is depressive or not.

To see the full code, check the notebook: 

https://github.com/viritaromero/Detecting-Depression-in-Tweets/blob/master/Depression_detection_tweets.ipynb

Datasets

Sentiment140

The Sentiment140 dataset contains 1,600,000 tweets extracted using the twitter API. The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment. It contains the following 6 fields:

    target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)
    ids: The id of the tweet ( 2087)
    date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
    flag: The query (lyx). If there is no query, then this value is NO_QUERY.
    user: the user that tweeted (robotickilldozr)
    text: the text of the tweet (Lyx is cool)

You can find the dataset here:

https://www.kaggle.com/kazanova/sentiment140

For my experiment, I just took a sample of 8,000 tweets with polarity of 4, the positive ones.

Web scraping depressive Tweets with TWINT

I didn’t find good quality and labeled datasets containing depressive tweets and some projects using a good dataset didn’t share the link due to privacy concerns.

Lucky me, found Twint, an advanced Twitter scraping tool written in Python that doesn’t use Twitter’s API, allowing you to scrape a user’s followers, following, Tweets and more while evading most API limitations.

You can find the tool here:

https://github.com/twintproject/twint


