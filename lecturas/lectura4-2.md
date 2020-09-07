# Critica: Document Clustering Based On Non-negative Matrix Factorization



Este paper trata sobre la tarea de realizar clúster de documentos por sus distintas categorías, esta practica se ha hecho cada vez mas relevante por lo que la investigación en este tema ha ido creciendo.

La principal novedad de este articulo es el uso de factorización matricial donde los vectores latentes son no negativos. esto dado que los autores creen que es razonable para categorizar documentos, donde esta categorización es la suma de distintas categorías. donde no tiene mucho sentido restarle una categoría. además esto le da la ventaja al método de tener vectores latentes que se asocian directamente a un clúster, donde en SVD se debe  realizar un paso extra de K-mean para encontrar los cluster.

Se ocupan dos fuentes de datos distintas y dos métricas de evaluación para cuatro distintos algoritmo. el orden de este paper me hizo creer que en un primer lugar su método no pudo vencer a NC por lo que recurrieron a usar la misma estrategia de considerar pesos y con esto pudieron finalmente vencerlo. aquí me falto una mejor explicación de cual es la función de estos pesos y porque son tan efectivos, tanto para NC como NMF-NCW ya que es muy relevante la diferencia en rendimiento que existe al considerarlos.

Por otro lado no me quedo conforme con la comparación que se hace versus el método de SVD ya que (excepto que AA y NMF sean SVD (cosa que nunca señala)) no se realiza una comparación en el rendimiento de estos métodos, solo se muestra que en en el espacio vectorial de NC realizar el clustering es mas directo, pero creo que perder esto por un método con mejor accuracy no es terrible.

Por ultimo tampoco quedo conforme con que no incluyan el costo de calcular la matriz de similitud, ya que es costoso computacionalmente y es un paso muy importante a la hora de querer implementar esto en producción.