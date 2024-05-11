# AVANCE 1: Sintesis-de-reuniones-con-IA-Equipo-31-TEC

# Proyecto: Síntesis de reuniones a través de la Inteligencia Artificial

## Introducción
Este documento presenta el primer avance del proyecto "Síntesis de reuniones a través de la Inteligencia Artificial" para SISTICA. El objetivo principal del proyecto es desarrollar una solución que permita sintetizar automáticamente la información de las reuniones entre SISTICA y sus clientes, capturando los detalles y requisitos clave para agilizar los procesos y mejorar la satisfacción del cliente.

## Análisis Exploratorio de Datos (EDA)

### 1. Descripción general de los datos
Para este proyecto, contamos con 20 archivos de texto en español, que pretenden actuar como las transcripciones de las reuniones entre SISTICA y sus clientes, que por motivos de privacidad de información no se pueden tener reales. La duración de las reuniones varía entre 15 minutos y 1 hora y 30 minutos.

### 2. Análisis de valores faltantes
Dado que los archivos son transcripciones completas de las reuniones, no se esperan valores faltantes en los datos de texto. Sin embargo, se realizará una verificación exhaustiva de los archivos para confirmar la integridad de los datos.

### 3. Estadísticas resumidas
- Número total de palabras: [Por definir]
- Número promedio de palabras por reunión: [Por definir]
- Duración promedio de las reuniones: [Por definir]

[Insertar histograma o gráfico de caja de la distribución de la duración de las reuniones](Pendiente)

### 4. Análisis de valores atípicos
En el contexto de las transcripciones de reuniones, los valores atípicos pueden referirse a reuniones excepcionalmente largas o cortas en comparación con la duración promedio. Se identificarán las reuniones que se desvían significativamente de la duración típica y se considerará si requieren un tratamiento especial durante el procesamiento.

### 5. Cardinalidad de las variables categóricas
En este caso, no hay variables categóricas explícitas en los datos de texto.

### 6. Distribución de los datos
Se realizará un análisis de la distribución de la longitud de las transcripciones (número de palabras) para determinar si hay sesgos o asimetrías en los datos. Si se observan distribuciones altamente sesgadas, se considerará la aplicación de transformaciones no lineales, como la escala logarítmica.

### 7. Tendencias temporales
No se dispone.

### 8. Correlación entre variables
En el contexto de las transcripciones de texto, no hay variables dependientes e independientes explícitas. Sin embargo, se explorará la correlación entre la duración de las reuniones y la longitud de las transcripciones para ver si existe alguna relación.

### 9. Clustering
Pendiente por ser analizado.

### 10. Desequilibrio de clases
En este caso, no hay una variable objetivo explícita con clases desequilibradas. Sin embargo, si se identifican ciertos tipos de reuniones (por ejemplo, reuniones de ventas, reuniones técnicas) durante el análisis, se evaluará si hay un desequilibrio en la representación de estos tipos.

## Fundamentos teóricos
El proyecto de síntesis de reuniones a través de la Inteligencia Artificial se basa en varios conceptos y técnicas clave:

- Procesamiento del Lenguaje Natural (NLP): Se utilizarán técnicas de NLP para analizar y comprender el contenido de las transcripciones de las reuniones, como la tokenización, la eliminación de palabras vacías y la lematización.

- Modelos de Lenguaje: Se emplearán modelos de lenguaje pre-entrenados, como BERT o GPT, para capturar la semántica y el contexto de las transcripciones y generar resúmenes coherentes.

- Algoritmos de Resumen Automático: Se aplicarán algoritmos de resumen automático, como TextRank o Sequence-to-Sequence, para identificar las oraciones más relevantes y generar resúmenes concisos de las reuniones.

Estas técnicas y enfoques permitirán sintetizar los audios largos de las reuniones en ideas concisas y capturar los detalles y requisitos clave para el equipo de SISTICA.

## Conclusión
Este primer avance del proyecto "Síntesis de reuniones a través de la Inteligencia Artificial" para SISTICA presenta un análisis exploratorio de datos inicial de las transcripciones de las reuniones. Se han identificado los pasos a seguir para completar el EDA.



# AVANCE 2: Sintesis-de-reuniones-con-IA-Equipo-31-TEC
# Proyecto: Síntesis de reuniones a través de la Inteligencia Artificial
### Instrucciones
En esta fase, conocida como ingeniería de características (FE - Feature Engineering):
## A Se aplicarán operaciones comunes para convertir los datos crudos del mundo real, en un conjunto de variables útiles para el aprendizaje automático. 
## Normalización
La normalización de texto es esencial en el campo del procesamiento de lenguaje natural para que las máquinas comprendan y analicen el lenguaje humano. Al estandarizar el texto, facilita la tarea de identificar componentes léxicos y realiza análisis lingüísticos.

La normalización de texto desempeña un papel significativo en el campo del machine learning y la inteligencia artificial. En el aprendizaje automático, los modelos a menudo trabajan con datos de texto para tareas como la clasificación de texto, la generación de lenguaje natural y la extracción de información. La normalización de texto asegura que los modelos funcionen de manera efectiva al proporcionar datos limpios y coherentes para el entrenamiento.

### ¿Cómo se realizará la normalización de texto?
1.	Conversión a minúsculas: Para asegurarnos de que todas las palabras se comparen de manera uniforme, es común convertir todo el texto a minúsculas. De esta manera, “Texto” y “texto” se considerarán iguales.
2.	Eliminación de caracteres especiales: Los caracteres especiales, como signos de puntuación o caracteres no alfabéticos, a menudo se eliminan o reemplazan por espacios en blanco.
3.	Eliminación de números: En algunos casos, los números no son relevantes para el análisis de texto por lo que se pueden eliminar.
4.	Tokenización: por medio del proceso de dividir el texto en palabras o tokens individuales. Esto permite analizar cada palabra por separado y es fundamental en el procesamiento de lenguaje natural.
5.	Eliminación de palabras vacías: Las palabras vacías, como “a”, “de” y “en”, se eliminan, ya que no aportan significado en muchos casos.
6.	Adicional se llevará a cabo la codificación mediante el estándar Unicode para la normalización de texto. Unicode es un sistema de codificación de caracteres que abarca la mayoría de los caracteres escritos utilizados en todo el mundo. Garantiza que los caracteres de diferentes idiomas se puedan representar de manera consistente en sistemas informáticos, lo que facilita la normalización de texto en varios idiomas, especialmente en aplicaciones globales y en el procesamiento de datos en diferentes lenguajes.



### Librería Spacy para la normalización de texto
Una herramienta valiosa para realizar la normalización de texto en programación es la librería Spacy. Spacy es una librería de procesamiento de lenguaje natural en Python que ofrece funciones avanzadas de tokenización, lematización y normalización de texto. 


## B. Además, se utilizarán métodos de filtrado para la selección de características y técnicas de extracción de características, permitiendo reducir los requerimientos de almacenamiento, la complejidad del modelo y el tiempo de entrenamiento.

El Análisis Semántico Latente (LSA) es una técnica computacional utilizada para analizar cómo se usan las palabras y los grupos de palabras en textos. 

El LSA se utiliza para responder preguntas como: ¿Cuál es el significado subyacente del texto? ¿Qué efecto tienen las palabras en el significado de los pasajes?
El lenguaje, especialmente en inglés, es complejo debido a que las palabras pueden tener múltiples significados. Por ejemplo, la palabra “caliente” puede significar cosas diferentes según el contexto.

### Método:
Se crea una matriz donde cada elemento muestra con qué frecuencia aparecen las palabras en un texto.
El LSA utiliza una técnica avanzada de álgebra matricial llamada Descomposición de Valores Singulares (SVD) para factorizar estas matrices.
Básicamente, el texto se convierte en matrices para representar pasajes, y cada celda de la matriz contiene el número de veces que aparece una palabra específica en un pasaje.
Luego, se factoriza la matriz para representar cada pasaje como un vector, donde el valor de cada vector es la suma de los vectores que representan sus palabras componentes.
Se utilizan productos de puntos o métricas similares para medir similitudes entre palabras y pasajes.

El análisis semántico latente (LSA) es una técnica estadística para analizar y modelar relaciones entre términos y documentos en un gran corpus de texto. Es una forma de reducción de la dimensionalidad que tiene como objetivo descubrir la estructura semántica subyacente del texto mediante la reducción de la dimensionalidad de los datos mientras se retiene la mayor cantidad de información relevante posible. LSA se usa ampliamente en aplicaciones de procesamiento de lenguaje natural (NLP), como agrupación de documentos, recuperación de información y clasificación de texto.

En esencia, LSA se basa en la suposición de que las palabras que se usan en contextos similares tienden a tener significados similares. LSA representa documentos como vectores en un espacio de alta dimensión, donde cada dimensión representa un término en el corpus. Las entradas en el vector representan la frecuencia de cada término en el documento. Luego, el algoritmo LSA transforma la matriz de documento de término en un espacio de menor dimensión al descomponerlo en sus valores singulares y vectores singulares constituyentes. La matriz resultante es una representación densa y de baja dimensión de los datos originales que captura las relaciones latentes entre los términos y los documentos.

Uno de los beneficios clave de LSA es que puede usarse para identificar relaciones semánticas entre palabras y documentos, incluso cuando esas relaciones no se expresan explícitamente en el texto. Por ejemplo, LSA se puede utilizar para identificar sinónimos, antónimos y otras relaciones semánticas entre palabras en función de sus patrones de concurrencia en el corpus. De manera similar, LSA se puede usar para identificar similitudes y diferencias entre documentos en función de su estructura semántica subyacente.

LSA tiene una amplia gama de aplicaciones en PNL. Una de sus aplicaciones más comunes es la recuperación de información, donde se utiliza para clasificar documentos en función de su relevancia para una consulta determinada. En este contexto, LSA se puede utilizar para identificar documentos que son semánticamente similares a la consulta, incluso si no contienen exactamente las mismas palabras clave. LSA también se puede utilizar para la clasificación de texto, donde se utiliza para clasificar documentos automáticamente en categorías predefinidas en función de su contenido semántico.

Flexibilidad y escalabilidad: NLP que requieren procesar grandes volúmenes de texto.

## Tokenización de texto con NLTK
La tokenización es el proceso de dividir un texto en unidades más pequeñas, como palabras o frases. NLTK proporciona una función de tokenización que nos permite dividir un texto en palabras individuales de manera sencilla

import nltk

nltk.download('punkt')

from nltk.tokenize import word_tokenize

text = "El procesamiento de lenguaje natural es fascinante."

tokens = word_tokenize(text)

print(tokens)

## Extracción de entidades nombradas con spaCy
Las entidades nombradas son fragmentos de texto que hacen referencia a personas, lugares, organizaciones, fechas, etc. SpaCy nos permite identificar y extraer entidades nombradas de un texto:

import spacy

nlp = spacy.load("es_core_news_sm")

text = "Juan trabaja en Google desde el año 2010."

doc = nlp(text)

for entity in doc.ents:
    print(entity.text, entity.label_)
