# Critica: Deep Learning based Recommender System: A Survey and New Perspectives.

En este estudio se presentan las principales técnicas de Deep learning y como estas son utilizadas en los sistemas recomendadores. La motivación nace de la gran velocidad a la que nuevas técnicas del área han emergido y la necesidad de catalogarlas todas para traer orden al área.

Primero se parte explicando las diferentes técnicas de Deep learning existentes y sus diferentes usos, luego para cada una de estas técnicas se explica como estas pueden ser usadas para sistemas recomendadores. Para esta semana leímos sobre tres técnicas. MLP, Autoencoders y CNNs.

MLP es la técnica original de Deep learning consiste en múltiples capas de perceptrones conectadas entre sí. El principal uso de esta técnica es para representar las relaciones no lineales entre los usuarios e ítems, relaciones que la factorización matricial no es capaz de captar, es por esto que es común encontrar un MLP con Factorización matricial en conjunto para hacer recomendación.

Los autoencoders que tiene dos principales usos, en primer lugar, para aprender atributos de los datos en dimensiones mas bajas, y para reconstruir datos de el input para entregarlos completos en el output. Es por esto que una manera muy natural para usar autoencoders es la de entregarle una matriz sparse y que este complete los elementos vacíos, de esta forma estos elementos ahora completos pueden ser usados como los ratings de recomendación.

Por ultimo los CNNs son ampliamente usados para el análisis de fotos, texto, videos, audio, etc. Por lo que son muy útiles para hacer recomendación con contexto, permite ahora a la hora de hacer recomendación procesar las imágenes de un item, o sus reviews por ejemplo, por lo que trae al mundo de la recomendación toda una gama de datos que antes era muy costosa de utilizar.

Como critica al paper es que intenta condensar mucha información en un texto corto, y de manera no tan clara, por lo que yo a veces me perdí con diversos métodos y técnicas que este presentaba. Aun así, creo que esta es la idea de este ya que presenta muchos artículos en donde ahondar en las cosas que este mismo explica, permitiendo al lector interesado poderse informarse en profundidad.

La verdad me parece un gran review, ya que concentra mucha información y permite a un lector no experto entrarse en el área de fondo y ver todas las posibilidades existentes.
