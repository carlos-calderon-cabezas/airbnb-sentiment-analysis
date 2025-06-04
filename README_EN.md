# Sentiment Analysis with Natural Language Processing Applied to Airbnb Reviews

[**Click here for the spanish version**](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/README.md)

![resized_image_250](https://github.com/user-attachments/assets/745d3055-36a5-4a3e-9741-8ea364b179dd)

**Welcome to my sentiment analysis project!** 😊🏖️😐🏄😠✈️😢

[Click here to view the project](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/airbnb_sentiment_analysis_EN.ipynb)

## Table of Contents

- [Project Description](#project-description)
- [Project Content](#project-content)
- [Usage Instructions](#usage-instructions)
- [Brief Summary of Conclusions and Recommendations](#brief-summary-of-conclusions-and-recommendations)

---

## Project Description

In this repository, I have developed a practical application with real data on sentiment analysis, which is part of natural language processing (NLP), a subset of artificial intelligence applications. This project also covers some fundamental concepts of data science, from data mining, data cleaning and preprocessing, data organization, and the development of artificial intelligence models from this data.

The main objective is to use artificial intelligence and natural language processing to help Airbnb accommodations understand their guests' opinions and improve their service. This is achieved through sentiment analysis, identifying patterns in reviews to suggest areas for improvement, thereby attracting more guests.

This project is entirely written in ***Python*** and developed in the ***Jupyter Notebook*** environment within the ***Google Colab*** cloud services platform.

To conduct this study, I obtained a sample of data from reviews left by guests at various accommodations offered on the ***Airbnb*** platform, focusing specifically on the Montañita resort in the Republic of Ecuador, which is visited annually by several thousand national and international tourists from various countries around the world.

It is important to mention that, since the Airbnb API is not publicly accessible and does not accept access requests at the time of this project, I had to perform manual data mining, which required a significant time investment at this stage. I had to devise a way using Python to process this unstructured information and convert it into a ***Pandas DataFrame*** for further processing. The code I created for this process is replicable for any number of reviews and accommodations from a plain text file.

Since reviews are available in multiple languages, including Spanish and English, I also translated guest reviews into a single language—English in this case—since the ***nltk*** library is optimized for natural language processing in English. Additionally, several reviews contain emojis, so it was necessary to convert them into equivalent words. As the next step, I removed unnecessary words for ***sentiment analysis*** with the help of the same ***nltk*** library.

Finally, I conducted the sentiment analysis, which takes the words found in each review and measures their polarity. Based on the number of words found for each category, a sentiment is assigned to the review. I present a confusion matrix at the end of this experiment, analyze the results obtained, and propose strategies that could be implemented by both hosts and the Airbnb platform itself if given the opportunity to discuss this with them.

## Project Content

- `airbnb_sentiment_analysis.ipynb`: Google Colab Jupyter Notebook written in Python.
- Folder `abb_reviews`, containing 10 files corresponding to 10 accommodations with guest reviews.
- Folder `output`, containing all the output files produced by this model:
  - `sentiment_matrix.xlsx`: Contains the actual sentiments, which were manually assigned, and the predicted sentiments by the model.
- Folder `translations`: Contains two files with translated reviews in both Spanish and English:

*Note: To avoid generating an API key in `Google Cloud Translate`, it is suggested to keep the `translations` folder. If you wish to perform translations using Google Cloud, you can safely delete this folder.*

## Usage Instructions

To use this project, follow these steps:

1. Clone the repository or download all files.
2. Ensure you have the required Python packages installed: `pandas`, `emoji`, `nltk`, `matplotlib`, and `seaborn`.
3. Open the `airbnb_sentiment_analysis.ipynb` file in your preferred working environment, such as `Jupyter Notebook`, `Google Colab`, `DataSpell`, among others.
4. Run the notebook cells to see the manual data mining and sentiment analysis performed.

No additional software installation or environment configuration is needed beyond having Jupyter and the previously mentioned Python libraries.

## Brief Summary of Conclusions and Recommendations

### Suggestions for Hosts

- Regarding positive comments, words such as "great", "good", "excellent", "comfortable", "clean", and "friendly" frequently appear. It is suggested that hosts continue implementing and improving good hygiene and cleanliness practices in their accommodations and maintain a friendly attitude towards guests to sustain and even increase booking volumes, benefiting both themselves and the platform.

- Regarding negative comments, words like "bad", "ugly", "terrible", "dirty" are quite common. Therefore, hosts should strive to create a positive experience by maintaining a welcoming and friendly environment. This includes promptly addressing guests' needs, valuing and respecting their different viewpoints. Regular inspections and maintenance are necessary to ensure all aspects of the stay meet or exceed expectations, preventing unfavorable reviews. This includes paying attention to aesthetics, keeping the property visually appealing, clean, and well-maintained. Optionally, updating the decor and furniture to create a more inviting space can reduce the likelihood of guests describing the property as "ugly" or "unpleasant".

  - Transparency is essential to avoid surprises. Providing detailed and accurate property descriptions and house rules can prevent guests from experiencing "shocks" or "inconveniences". Finally, paying attention to cleanliness, especially in areas like bathrooms and kitchens, will ensure guests do not describe the property as "dirty" or "unclean".

- As the next phase, I plan to discuss with various Airbnb hosts in Montañita about the reviews, seeking together areas for improvement. A negative impression from guests can sometimes affect not only the hosts but also the city and even the country. Considering many tourists visit Ecuador solely to visit certain destinations like Montañita, it is also the hosts' responsibility to ensure guests leave with the best possible image of the country.

### Commercial Value of the Analysis

- If considering selling this product to the Airbnb platform in the future, my main recommendation would be to implement a bot that constantly runs this model. If it detects one or several negative words mentioned in Montañita's accommodations, an alert should be sent to Airbnb's Support Team to immediately communicate with the involved host(s) to inform them and work together to offer a better guest experience. This, in turn, will further increase guests' trust in the Airbnb platform in Montañita.
- For positive comments, as mentioned earlier, it is recommended to provide a small financial incentive to hosts with a considerable number of consecutive positive reviews. The bot running this model could be helpful here as well. One way to provide this incentive could be that Airbnb covers the total or part of the service fee, cleaning fees, among others, for these specific cases. This would encourage guests to choose the better-reviewed accommodation over others, increasing sales for that particular host and the platform itself.
