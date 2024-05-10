**¡Bienvenidos a mi repositorio sobre an&aacute;lisis de sentimientos! / Welcome to my sentiment analysis open repository!**

<img src="https://i.imgur.com/4I0Em2T.png" alt="Project Collage" width="50%">

[**Click here for the english version**](#english) | [**Haz clic aquí para la versión en español**](#español)

---

# English

In this repository I have developed a practical application with real data on sentiment analysis, which is part of natural language processing (NLP), which in turn is part of the applications that can be developed with artificial intelligence. In this project I also cover some of the fundamental concepts of data science, from data mining, through data cleaning and preprocessing, its organization, and the development of artificial intelligence models from them.

The main goal is to use artificial intelligence and natural language processing to help Airbnb properties located in Montañita to understand their guests' opinions and improve their service. This is achieved through sentiment analysis, identifying patterns in comments to suggest areas for improvement to attract more guests.

This project is written entirely in the ***Python*** programming language, and is developed in the ***Jupyter Notebook*** environment within the ***Google Colab*** cloud services platform.

To carry out this study, I obtained a sample of data from reviews left by guests of different accommodations that are offered by the temporary accommodation platform ***Airbnb***, with a specific focus on the Montañita spa located in the Republic of Ecuador, which is visited every year by several thousand national and foreign tourists from various countries around the world.

It is important to tell you that, because the Airbnb API is not accessible to the general public and they do not receive access requests at the time of carrying out this project, I had to perform data mining manually, which meant a considerable investment of time at this stage, since I had to devise, using Python, a way to process said unstructured information to convert it into a ***Pandas DataFrame*** that can be processed later. The code I created for that process is replicable for any number of reviews and accommodations that come from a plain text file.

Because there are reviews in multiple languages, including Spanish and English, I have also translated guest reviews into a single language - which in this case is English - since the library ***nltk*** It is optimized for natural language processing in the English language. Additionally, several of the comments contain emojis so it was necessary to convert them into equivalent words. As a next step, I removed the words that were not necessary for the ***sentiment analysis*** with the help of the same ***nltk*** library.

Lastly, I performed sentiment analysis, which takes the words found in each review and measures their polarity, so depending on the number of words found for each category, a sentiment is returned for this comment. At the end I show a confusion matrix with the result of this experiment.

---

# Español

En este repositorio he desarrollado una aplicación práctica con datos reales sobre en análisis de sentimientos, el cual forma parte del procesamiento del lenguaje natural (NLP), mismo que a su vez forma parte de las aplicaciones que se pueden desarrollar con inteligencia artificial. En este proyecto también cubro algunos de los conceptos fundamentales de la ciencia de datos, desde la minería de datos, pasando por la limpieza y el preprocesamiento de datos, su organización, y el desarrollo de modelos de inteligencia artificial a partir de estos.

El objetivo principal consiste en utilizar inteligencia artificial y procesamiento del lenguaje natural para ayudar a los alojamientos ofrecidos en Airbnb a comprender las opiniones de sus huéspedes y mejorar su servicio. Esto se logra mediante el análisis de sentimientos, identificando patrones en los comentarios para sugerir áreas de mejora y así atraer a más huéspedes.

Este proyecto está escrito por completo en el lenguaje de programación ***Python***, y se desarrolla en el entorno de ***Jupyter Notebook*** dentro de la plataforma de servicios en la nube de ***Google Colab***.

Para realizar el presente estudio obtuve una muestra de datos provenientes de reseñas dejadas por huéspedes de diferentes alojamientos que son ofertados por la plataforma de alojamientos temporales ***Airbnb***, con un enfoque específico en el balneario de Montañita ubicada en la República de Ecuador, mismo que es visitado al año por varios miles de turistas tanto nacionales como extranjeros provenientes de varios países al rededor del mundo.

Es importante para comentarles que, debido a que la API de Airbnb no es accesible al público en general y tampoco reciben solictudes de acceso al momento de realizar este proyecto, tuve que realizar la minería de datos de manera manual, lo cual significó una inversión considerable de tiempo en esta etapa, ya que tuve que idear mediante Python una manera de procesar dicha información no estructurada para convertirla en un ***DataFrame de Pandas*** que pueda ser procesado posteriormente. El código que creé para dicho proceso es replicable para cualquier número de reseñas y alojamientos que provienen de un archivo de texto plano.

Debido a que existen reseñas en múltiples idiomas, incluidos español e inglés, he realizado también la traducción de las reseñas de los huéspedes a un úmico idioma -que en este caso es el inglés-, ya que la librería ***nltk*** está optimizada para el procesamiento del lenguaje natural en idioma inglés. Adicionalmente, varios de los comentarios contienen emojis por lo cual fue necesario convertirlos en palabras equivalentes. Como siguiente paso, eliminé las palabras que no eran necesarias para el ***análisis de sentimientos*** con la ayuda de la misma librería ***nltk***.

Por último, realicé el análisis de sentimientos, mismo que toma las palabras que encuentra en cada reseña y mide su polaridad, por lo cual según la cantidad de palabras que encuentre para cada categoría, se devuelve un sentimiento para este comentario. Muestro al final una matriz de confusión con el resultado de este experimento.
