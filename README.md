# Análisis de sentimientos con Procesamiento de Lenguaje Natural aplicado a reseñas de Airbnb 

[**Click here for the english version**](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/README_EN.md)

![resized_image_250](https://github.com/user-attachments/assets/745d3055-36a5-4a3e-9741-8ea364b179dd)

**¡Bienvenidos a mi proyecto sobre análisis de sentimientos!** 😊🏖️😐🏄😠✈️😢

[Click aquí para ver el proyecto](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/airbnb_sentiment_analysis.ipynb) / [Click here to view the project](https://github.com/carlos-calderon-cabezas/airbnb-sentiment-analysis/blob/main/airbnb_sentiment_analysis_EN.ipynb)

## Tabla de Contenidos

- [Descripción del proyecto](#descripción-del-proyecto)
- [Contenido del proyecto](#contenido-del-proyecto)
- [Instrucciones de uso](#instrucciones-de-uso)
- [Breve resumen de conclusiones y recomendaciones](#breve-resumen-de-conclusiones-y-recomendaciones)


---

## Descripción del proyecto

En este repositorio he desarrollado una aplicación práctica con datos reales sobre en análisis de sentimientos, el cual forma parte del procesamiento del lenguaje natural (NLP), mismo que a su vez forma parte de las aplicaciones que se pueden desarrollar con inteligencia artificial. En este proyecto también cubro algunos de los conceptos fundamentales de la ciencia de datos, desde la minería de datos, pasando por la limpieza y el preprocesamiento de datos, su organización, y el desarrollo de modelos de inteligencia artificial a partir de estos.

El objetivo principal consiste en utilizar inteligencia artificial y procesamiento del lenguaje natural para ayudar a los alojamientos ofrecidos en Airbnb a comprender las opiniones de sus huéspedes y mejorar su servicio. Esto se logra mediante el análisis de sentimientos, identificando patrones en los comentarios para sugerir áreas de mejora y así atraer a más huéspedes.

Este proyecto está escrito por completo en el lenguaje de programación ***Python***, y se desarrolla en el entorno de ***Jupyter Notebook*** dentro de la plataforma de servicios en la nube de ***Google Colab***.

Para realizar el presente estudio obtuve una muestra de datos provenientes de reseñas dejadas por huéspedes de diferentes alojamientos que son ofertados por la plataforma de alojamientos temporales ***Airbnb***, con un enfoque específico en el balneario de Montañita ubicada en la República de Ecuador, mismo que es visitado al año por varios miles de turistas tanto nacionales como extranjeros provenientes de varios países al rededor del mundo.

Es importante para comentarles que, debido a que la API de Airbnb no es accesible al público en general y tampoco reciben solictudes de acceso al momento de realizar este proyecto, tuve que realizar la minería de datos de manera manual, lo cual significó una inversión considerable de tiempo en esta etapa, ya que tuve que idear mediante Python una manera de procesar dicha información no estructurada para convertirla en un ***DataFrame de Pandas*** que pueda ser procesado posteriormente. El código que creé para dicho proceso es replicable para cualquier número de reseñas y alojamientos que provienen de un archivo de texto plano.

Debido a que existen reseñas en múltiples idiomas, incluidos español e inglés, he realizado también la traducción de las reseñas de los huéspedes a un úmico idioma -que en este caso es el inglés-, ya que la librería ***nltk*** está optimizada para el procesamiento del lenguaje natural en idioma inglés. Adicionalmente, varios de los comentarios contienen emojis por lo cual fue necesario convertirlos en palabras equivalentes. Como siguiente paso, eliminé las palabras que no eran necesarias para el ***análisis de sentimientos*** con la ayuda de la misma librería ***nltk***.

Por último, realicé el análisis de sentimientos, mismo que toma las palabras que encuentra en cada reseña y mide su polaridad, por lo cual según la cantidad de palabras que encuentre para cada categoría, se devuelve un sentimiento para este comentario. Muestro al final una matriz de confusión con el resultado de este experimento y realizo un análisis con los resultados obtenidos y propongo estrategias que podrían ser implementadas tanto por anfitriones, como por la propia plataforma de Airbnb en caso de tener el algún momento la oportunidad de conversar con ellos.

## Contenido del proyecto

- `airbnb_sentiment_analysis.ipynb`: Jupyter Notebook de Google Colab escrito en Python.
- Carpeta `abb_reviews`, mismo que contiene los 10 archivos, correspondientes a 10 alojamientos a los cuales los huéspedes dejaron reseñas.
- Carpeta `output`, la cual contiene todos los archivos de salida que produce este modelo:
  - `matriz_sentimientos.xlsx`: Contiene los sentimientos reales, los cuales fueron asignados manualmente y los sentimientos predichos por el modelo.
- Carpeta `translations`: Contiene dos archivos con reseñas traducidas tanto al español como al inglés:

*Nota: Para que no tengas que generar una clave API en `Google Cloud Translate`, se sugiere que conserves la carpeta `translations`. Si deseas realizar las traducciones usando la nube de Google, puedes borrar de manera segura esta carpeta.*

## Instrucciones de uso

Para utilizar este proyecto es necesario seguir estos pasos:

1. Clonar el repositorio o descargar todos los archivos.
2. Asegurarse de tener instalados los paquetes de Python que se usan en el proyecto: `pandas`, `emoji`, `nltk`, `matplotlib` y `seaborn`.
3. Abrir el archivo `airbnb_sentiment_analysis.ipynb` en cualquier entorno de trabajo de tu preferencia, puede ser `Jupyter Notebook`, `Google Colab`, `DataSpell`, entre otros.
4. Ejecutar las celdas del notebook para ver la minería manual de datos y el análisis de sentimientos que he realizado.

No es necesario instalar software adicional ni configurar el entorno más allá de tener Jupyter y las librerías de Python previamente descritas.

## Breve resumen de conclusiones y recomendaciones

### Sugerencias para anfitriones

- En cuanto a comentarios positivos, se ve que se repiten palabras tales como "genial", "bueno", "excelente", "comfortable", "limpio, "amigable", por lo cual se sugiere a los anfitriones continuar implementando y mejorando buenas prácticas de higiene y limpieza en sus alojamientos, así como mostrarse amigables con los huéspedes a fin de mantener y incluso incrementar el volumen de reservas, lo cual beneficia no solo a ellos, pero también a la plataforma.

- En cuanto a los comentarios negativos, son bastante comunes palabras tales como "malo", "feo", "terrible", "sucio", entre otras. Es por esta razón que los anfitriones deben esforzarse por crear una experiencia positiva manteniendo un ambiente acogedor y amigable, para ello se debe atender las necesidades de los huéspedes de manera pronta, valoradondo y respetando sus diferentes puntos de vista. Se deben además realizar inspecciones y mantenimientos regulares para asegurarse de que todos los aspectos de la estadía cumplan o superen las expectativas a fin de prevenir reseñas desfavorables. Esto incluye prestar atención a la estética, manteniendo la propiedad visualmente atractiva, limpia y bien cuidada. Además se podría opcionalmente actualizar la decoración y el mobiliario para crear un espacio más acogedor, reduciendo la probabilidad de que los huéspedes describan la propiedad como "fea" o "desagradable".

  - La transparencia es esencial para evitar sorpresas. Proporcionar descripciones detalladas y precisas de la propiedad y cualquier regla de la casa puede prevenir que los huéspedes experimenten "sobresaltos" o "inconvenientes". Finalmente, prestar atención a los detalles de la limpieza, especialmente en áreas como baños y cocinas, asegurará que los huéspedes no describan la propiedad como "sucia" o llena de "suciedad".

- Como próxima fase, me planteo conversar con diferentes anfitriones de Airbnb en Montañita para conversar con ellos sobre las reseñas, para buscar en conjunto áreas de mejora, porque al llevarse los huéspedes una mala impresión de un alojamiento, puede que en algunos casos no solo queden mal los anfitriones, pero también la ciudad e incluso el país, considerando que hay bastantes turistas que visitan Ecuador únicamente por ir a un cierto destino, como en este caso lo es Montañita, y es también responsabilidad de los anfitriones que los huéspedes se lleven la mejor imagen posible del país.

### Valor Comercial del Análisis
- En caso de querer venderle en algún punto en el futuro este producto a la plataforma de Airbnb, mi principal recomendación para ellos sería que implementar un bot que ejecute constantemente este modelo, y en caso de que se detecte que una o varias de las palabras negativas ya mancionadas en los alojamientos de Montañita, se mande una alerta al Equipo de Soporte de Airbnb, para que estos se comuniquen de inmedaito con el anfitrión o anfitriones involucrados para informar de lo sucedido y puedan trabajar en conjunto para ofrecer una mejor experiencia de cliente al huésped, lo que su vez incrementará aún más la confianza de estos en la plataforma de Airbnb en Montañita.
- En cuanto a los comentarios positivos, tal como se mencionó previamente también, se recomienda a la plataforma brindar un pequeño incentivo económico a los anfitriones que tengan un número considerable de reseñas positivas seguidas, para lo cual el bot que corra este modelo podría ser también de ayuda. Una de las maneras de otorgar dicho incentivo podría ser que Airbnb asuma para esos casos puntuales, el total o parte de la tarifa de servicio, gastos de limpieza entre otros, con lo cual se incentiva a que el huésped elija ese alojamiento con mejores reseñas en lugar de otro, y con ello aumente las ventas, tanto para ese anfitrión en cuestión como para la plataforma en sí.
