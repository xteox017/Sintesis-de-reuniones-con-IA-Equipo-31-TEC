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
