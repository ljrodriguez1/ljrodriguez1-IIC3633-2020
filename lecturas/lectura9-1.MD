# Critica: Multi-armed recommender system bandit ensembles.

El articulo presenta una estrategia de reinforcement learning para la creación de sistemas recomendadores híbridos que ocupen múltiples algoritmos para generar sus recomendaciones. Dice ser uno de los primeros en el área en ocupar el concepto de bandits para recomendar.

La motivación para usar este método resulta de que en producción los sistemas recomendadores deben actualizarse constantemente a medida que los usuarios e ítems cambian. Ya que diferentes algoritmos pueden presentar falencias o sesgos que no se dan a conocer de inmediato.

En este estudio se uso 3 algoritmos para ser combinados, estos se combinaron con dos bandits, e-greedy y Thompson sampling bandit. Ambos mostraros ser mejor que los ensambles dinámicos y que los tres algoritmos por sí solos.

La implementación de este algoritmo no se muestra en el paper lo cual lo encuentro insuficiente ya que este es un articulo relativamente corto y se podría haber ahondado mas en este tema, aun así, se entrega un link a github donde podemos observar la implementación y reproducir estos resultados.

También considero que se fue poco explorador en el ámbito de escoger distintos bandits ya que ambos que escogieron presentan un comportamiento bastante parecido, escogiendo en primer lugar most-popular y como en la etapa 50 cambiando a matrix factorization. Y siempre tomando muy poco en cuenta User-Knn. 

Esto me deja con las ganas de explorar como seria esta distribución si es que existieran mas algoritmos recomendadores, y distintos bandits, ¿existirá una mezcla que permita una elección de los algoritmos más homogénea?
