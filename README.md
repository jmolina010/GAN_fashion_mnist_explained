# GAN_fashion_mnist_explained

## Jerónimo Molina, noviembre de 2020

## Este notebook trata de explicar la filosofía y objetivo de las redes GAN -Generative Adversarial Networks- a partir de un ejemplo básico que genera imágenes de prendas de vestir y complementos basadas en el conjunto Fashion MNIST

**El código de este notebook está basado en un ejemplo del libro Python Deep Learning Introducción práctica con Keras y TensorFlow 2**, del profesor Jordi Torres.

### Introducción a las GAN

#### Las GAN son pares de redes neuronales que compiten entre sí para alcanzar un objetivo de generación de contenido, tal que, una, la generadora, precisamente se encarga de generar (imágenes vídeo, texto audio,...lo que sea) a partir de, incialmente, datos aleatorios, mientras que la otra, la discriminadora, analiza la información generada por la primera y decide si es un dato real o falso apoyándose en datos reales.

#### Se trata de dos redes que aprenden a la par y compiten entre sí, "jugando al gato y al ratón". El juego termina cuando la discriminadora no es capaz de distinguir entre los datos reales y los generados por la generadora. En ese momento, y si convergen de forma paralela (una no aprende mucho más rápido que la otra), la red generadora, si tiene un buen diseño, estará generando una salida lo suficientemente buena como para que no se distinga de la realidad (al menos según la red discriminadora).

#### Si ambas reden neuronales tienen una arquitectura suficientemente buena, se pueden conseguir grandes resultados.

#### En este notebook no nos vamos a centrar en crear una arquitectura de redes elaborada, sino en generar un modelo de GAN que permita explicar los conceptos subyacentes

#### La introducción y explicaciones en mayor detalle puede encontrarlas en el notebook, junto al código, en cada celda.

#### Enjoy the code!
