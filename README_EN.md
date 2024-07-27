**Welcome to my sentiment analysis open repository!**

<img src="https://i.imgur.com/4I0Em2T.png" alt="Project Collage" width="50%">

In this repository I have developed a practical application with real data on sentiment analysis, which is part of natural language processing (NLP), which in turn is part of the applications that can be developed with artificial intelligence. In this project I also cover some of the fundamental concepts of data science, from data mining, through data cleaning and preprocessing, its organization, and the development of artificial intelligence models from them.

The main goal is to use artificial intelligence and natural language processing to help Airbnb properties located in Montañita to understand their guests' opinions and improve their service. This is achieved through sentiment analysis, identifying patterns in comments to suggest areas for improvement to attract more guests.

This project is written entirely in the ***Python*** programming language, and is developed in the ***Jupyter Notebook*** environment within the ***Google Colab*** cloud services platform.

To carry out this study, I obtained a sample of data from reviews left by guests of different accommodations that are offered by the temporary accommodation platform ***Airbnb***, with a specific focus on the Montañita spa located in the Republic of Ecuador, which is visited every year by several thousand national and foreign tourists from various countries around the world.

It is important to tell you that, because the Airbnb API is not accessible to the general public and they do not receive access requests at the time of carrying out this project, I had to perform data mining manually, which meant a considerable investment of time at this stage, since I had to devise, using Python, a way to process said unstructured information to convert it into a ***Pandas DataFrame*** that can be processed later. The code I created for that process is replicable for any number of reviews and accommodations that come from a plain text file.

Because there are reviews in multiple languages, including Spanish and English, I have also translated guest reviews into a single language - which in this case is English - since the library ***nltk*** It is optimized for natural language processing in the English language. Additionally, several of the comments contain emojis so it was necessary to convert them into equivalent words. As a next step, I removed the words that were not necessary for the ***sentiment analysis*** with the help of the same ***nltk*** library.

Lastly, I performed sentiment analysis, which takes the words found in each review and measures their polarity, so depending on the number of words found for each category, a sentiment is returned for this comment. At the end I show a confusion matrix with the result of this experiment.