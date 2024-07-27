**¡Bienvenidos a mi repositorio sobre an&aacute;lisis de sentimientos! / Welcome to my sentiment analysis open repository!**

<img src="https://github.com/user-attachments/assets/d638e6c4-3821-4e5b-96d7-4c22b023380a" alt="Project Collage" width="50%">

[**Click here for the english version**](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/README_EN.md)

---


En este repositorio he desarrollado una aplicación práctica con datos reales sobre en análisis de sentimientos, el cual forma parte del procesamiento del lenguaje natural (NLP), mismo que a su vez forma parte de las aplicaciones que se pueden desarrollar con inteligencia artificial. En este proyecto también cubro algunos de los conceptos fundamentales de la ciencia de datos, desde la minería de datos, pasando por la limpieza y el preprocesamiento de datos, su organización, y el desarrollo de modelos de inteligencia artificial a partir de estos.

El objetivo principal consiste en utilizar inteligencia artificial y procesamiento del lenguaje natural para ayudar a los alojamientos ofrecidos en Airbnb a comprender las opiniones de sus huéspedes y mejorar su servicio. Esto se logra mediante el análisis de sentimientos, identificando patrones en los comentarios para sugerir áreas de mejora y así atraer a más huéspedes.

Este proyecto está escrito por completo en el lenguaje de programación ***Python***, y se desarrolla en el entorno de ***Jupyter Notebook*** dentro de la plataforma de servicios en la nube de ***Google Colab***.

Para realizar el presente estudio obtuve una muestra de datos provenientes de reseñas dejadas por huéspedes de diferentes alojamientos que son ofertados por la plataforma de alojamientos temporales ***Airbnb***, con un enfoque específico en el balneario de Montañita ubicada en la República de Ecuador, mismo que es visitado al año por varios miles de turistas tanto nacionales como extranjeros provenientes de varios países al rededor del mundo.

Es importante para comentarles que, debido a que la API de Airbnb no es accesible al público en general y tampoco reciben solictudes de acceso al momento de realizar este proyecto, tuve que realizar la minería de datos de manera manual, lo cual significó una inversión considerable de tiempo en esta etapa, ya que tuve que idear mediante Python una manera de procesar dicha información no estructurada para convertirla en un ***DataFrame de Pandas*** que pueda ser procesado posteriormente. El código que creé para dicho proceso es replicable para cualquier número de reseñas y alojamientos que provienen de un archivo de texto plano.

Debido a que existen reseñas en múltiples idiomas, incluidos español e inglés, he realizado también la traducción de las reseñas de los huéspedes a un úmico idioma -que en este caso es el inglés-, ya que la librería ***nltk*** está optimizada para el procesamiento del lenguaje natural en idioma inglés. Adicionalmente, varios de los comentarios contienen emojis por lo cual fue necesario convertirlos en palabras equivalentes. Como siguiente paso, eliminé las palabras que no eran necesarias para el ***análisis de sentimientos*** con la ayuda de la misma librería ***nltk***.

Por último, realicé el análisis de sentimientos, mismo que toma las palabras que encuentra en cada reseña y mide su polaridad, por lo cual según la cantidad de palabras que encuentre para cada categoría, se devuelve un sentimiento para este comentario. Muestro al final una matriz de confusión con el resultado de este experimento y realizo un análisis con los resultados obtenidos y propongo estrategias que podrían ser implementadas tanto por anfitriones, como por la propia plataforma de Airbnb en caso de tener el algún momento la oportunidad de conversar con ellos.
