# Análisis Exploratorio de Datos (EDA) – Productos Retail Flipkart

## Autor
*Alan Cuero*  
Analista de Datos Junior | Interés en Datos e Inteligencia Artificial  


## Descripción del Proyecto

Este proyecto presenta un *Análisis Exploratorio de Datos (EDA)* realizado sobre un conjunto de datos de productos minoristas de Flipkart.  
El objetivo principal es *analizar precios, descuentos, calificaciones de clientes y comportamiento de ventas, con el fin de generar **insights útiles para la toma de decisiones de negocio en e-commerce*.

El análisis sigue un flujo completo de trabajo profesional, incluyendo limpieza de datos, validación, visualización y síntesis de resultados.


## Objetivos del Análisis

- Comprender la estructura y calidad del dataset
- Analizar la distribución de precios
- Evaluar el comportamiento de precios por categoría
- Analizar el impacto de los descuentos en las ventas
- Explorar la relación entre precio y satisfacción del cliente
- Generar conclusiones claras orientadas al negocio


## Descripción del Dataset

- *Fuente:* Flipkart Retail Products Dataset  
- *Registros:* 80.000 productos  
- *Columnas:* 25 variables  
- *Formato:* CSV  

### Variables clave:
- price: precio original del producto  
- discount_percent: porcentaje de descuento  
- final_price: precio final de venta  
- units_sold: unidades vendidas  
- rating: calificación del producto (1–5)  
- review_count: número de reseñas  
- category, brand, seller_city: variables de segmentación  



## Herramientas Utilizadas

- *Python 3*
- *Pandas* – limpieza y manipulación de datos  
- *Matplotlib* – visualización de datos  
- *VS Code + Jupyter Notebook* – entorno de desarrollo  
- *Git & GitHub* – control de versiones y portafolio  

---

## Limpieza y Preparación de Datos

Durante esta fase se realizaron las siguientes acciones:

- Conversión de la variable listing_date a formato de fecha
- Tratamiento de valores nulos en la columna size
- Validación de coherencia entre precio, descuento y precio final
- Verificación de tipos de datos y estructura general

El dataset presenta *alta calidad de datos*, sin inconsistencias críticas que afecten el análisis.


## Distribución de Precios

### ¿Qué se analizó?
Se evaluó la distribución general de los precios de los productos disponibles en el marketplace para entender su rango y comportamiento.

### Observaciones principales
- Rango de precios aproximado: *200 – 60.000*
- El precio promedio es muy cercano a la mediana
- No se identificaron valores extremos irreales

### ¿Qué significa esto para el negocio?
El marketplace ofrece productos en distintos rangos de precio, atendiendo a diferentes tipos de clientes, con una distribución estable y sin anomalías relevantes.


## Precios por Categoría

### ¿Qué se analizó?
Se compararon los precios de los productos entre las distintas categorías del marketplace para identificar diferencias relevantes en su comportamiento.

### Observaciones principales
- Todas las categorías presentan distribuciones de precios muy similares
- Las medianas, rangos y niveles de variabilidad son comparables entre categorías

### ¿Qué significa esto para el negocio?
El catálogo de productos se encuentra balanceado en términos de precios entre categorías.  
Esto facilita análisis comparativos, aunque puede no reflejar completamente el comportamiento de un mercado real, donde algunas categorías suelen ser más costosas que otras.

## Impacto del Descuento en las Ventas

En esta sección se analiza la relación entre los *niveles de descuento* aplicados y el *comportamiento de las ventas*, con el objetivo de identificar si el descuento actúa como un factor determinante en el volumen de ventas dentro del dataset.

### Análisis General

A partir del análisis exploratorio de los datos, se observa que las *ventas promedio se mantienen relativamente estables a lo largo de los distintos rangos de descuento. Esto sugiere que las variaciones en el porcentaje de descuento **no producen cambios significativos* en el volumen promedio de ventas.

Asimismo, *no se identifica una relación directa o proporcional* entre un mayor nivel de descuento y un incremento en las ventas. En varios escenarios, aumentos en el descuento no se traducen en un mayor volumen de ventas, lo que indica que el efecto del descuento es limitado dentro de este conjunto de datos.

### Interpretación

Este comportamiento puede estar influenciado por otros factores que no dependen exclusivamente del descuento, tales como:

- Tipo o categoría del producto.
- Preferencias y fidelidad del cliente.
- Percepción del valor del producto.
- Factores temporales o estacionales.
- Estrategias de precios previamente establecidas.

Estos elementos podrían tener un impacto mayor en la decisión de compra que el descuento en sí.

### Insight Principal

> El descuento no es el principal factor que impulsa las ventas en este dataset.

Los resultados sugieren que *otras variables juegan un papel más relevante* en el comportamiento de las ventas. Por lo tanto, se recomienda complementar este análisis incorporando más variables y profundizando en su interacción para obtener una visión más completa y precisa del fenómeno.

---

## Relación entre Precio y Calificación

En esta sección se analiza la relación entre el *precio de los productos* y su *calificación (rating)*, con el fin de evaluar si el precio actúa como un indicador directo de la satisfacción del cliente.

### Análisis General

El análisis exploratorio muestra una *alta dispersión de las calificaciones a lo largo de todo el rango de precios*. Productos con precios bajos, medios y altos presentan calificaciones tanto altas como bajas, lo que indica un comportamiento heterogéneo en la percepción del cliente.

Adicionalmente, *no se identifica una tendencia clara* que sugiera que un mayor precio esté asociado sistemáticamente con mejores calificaciones. De manera similar, precios más bajos no implican necesariamente una peor evaluación por parte de los usuarios.

### Interpretación

Estos resultados sugieren que el *precio, por sí solo, no es un factor determinante de la satisfacción del cliente*. La percepción de calidad parece estar influenciada por múltiples variables adicionales, entre ellas:

- Expectativas previas del cliente.
- Reputación y posicionamiento de la marca.
- Experiencia de uso del producto o servicio.
- Relación entre precio y valor percibido.
- Servicio postventa y atención al cliente.

Por lo tanto, el precio debe entenderse como *un componente más dentro de un conjunto de factores* que influyen en la evaluación final del usuario.

### Insight Clave

> El precio no es un predictor directo de la satisfacción del cliente.

Este hallazgo indica que *incrementar el precio no garantiza una mejor percepción del producto*, y que estrategias centradas únicamente en el precio pueden ser insuficientes para mejorar la experiencia del cliente. Se recomienda complementar este análisis con variables cualitativas y de experiencia para obtener una visión más integral.



## Resumen de Hallazgos Clave

1. El dataset es consistente y bien estructurado.
2. Los precios no presentan valores atípicos extremos.
3. Las categorías muestran comportamientos de precio similares.
4. Los descuentos no tienen un impacto significativo en el volumen promedio de ventas.
5. Un mayor precio no garantiza una mejor calificación del producto.
6. La satisfacción del cliente depende de múltiples factores no relacionados directamente con el precio.


## Conclusiones

Este proyecto demuestra un flujo completo de análisis de datos, desde la preparación hasta la generación de insights de negocio.  
Los resultados evidencian la importancia de *analizar los datos antes de asumir relaciones directas*, como que mayores precios o mayores descuentos siempre generan mejores resultados.

El EDA se confirma como una herramienta fundamental para la toma de decisiones basadas en datos en entornos de comercio electrónico.


## Trabajo Futuro

- Segmentación por categoría y ciudad
- Análisis de correlación multivariable
- Modelos predictivos de ventas
- Dashboards interactivos (Power BI / Plotly)


##  Estructura del Repositorio

el proyecto esta organizado de esta manera 

flipkart-data-analysis/
│
├── Data/
│   └── flipkart.csv
│
├── notebooks/
│   └── 01_exploratory_analysis.ipynb
│
└── README.md

