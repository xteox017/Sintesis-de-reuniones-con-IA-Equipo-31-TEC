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
## Instrucciones
En esta fase, conocida como ingeniería de características (FE - Feature Engineering):
#### A Se aplicarán operaciones comunes para convertir los datos crudos del mundo real, en un conjunto de variables útiles para el aprendizaje automático. 
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



## Librería Spacy para la normalización de texto
Una herramienta valiosa para realizar la normalización de texto en programación es la librería Spacy. Spacy es una librería de procesamiento de lenguaje natural en Python que ofrece funciones avanzadas de tokenización, lematización y normalización de texto. 
