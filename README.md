# AeroFeel
###### by: Datahacks
-----------------------

El mercado aéreo comercial de México es altamente competitivo, lo que hace que la retención de clientes sea un aspecto crucial para alcanzar el éxito en este sector.

## Reto

VivaAerobus nos entregó un dataset en formato xlsx con 4 hojas, las cuáles están separadas por el punto en el que se recabó la opinión del cliente (paypoint). Este dataset con aproximadamente 76 mil registros en total, fue utilizado para el entrenamiento y evaluación de un modelo NLP, sin embargo, este notebook está creado con el objetivo de introducir la información que se recaba día con día. 

## Solución

Para la solución del reto decidimos utiizar DistilBERT, que es una versión más ligera y rápida del modelo original BERT, el cuuál es un modelo de procesamiento del lenguaje natural. 

Utilizamos este modelo para un análisis de sentimiento, pero, para realizar el fine-tuning, comparamos la calificación dada por el cliente con el sentimiento dado por el modelo, para después compararlo en una matriz de confusión.

Posteriormente, los comentarios se clasifican en las diferentes áreas de interés para la aerolínea con base en palabras clave; finalmente, se hace una limpieza de palabras altisonantes.

## Resultados

Con un promedio de 83% de precisión en los conjuntos de validación, tenemos un análisis de sentimiento satisfactorio gracias a nuestro modelo.

Para este punto, en el dataset final ya tenemos el paypoint, sentimiento y clasificacón, así como todos los otros campos previamente dados. 

Con esta información, se le permite a la aerolínea personalizar la búsqueda de comentarios ya sea por área, sentimiento, clasificación y hasta rango de fechas, con el objetivo de enfocarse específicamente en las áreas de oportunidad.
