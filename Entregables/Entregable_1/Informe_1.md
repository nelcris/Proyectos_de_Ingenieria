<p align="center">
  <img src="https://github.com/JefHuiza/Fundamentos-de-Dise-o/assets/156036185/d3c66dfb-5faa-419b-bf1b-d897ea110ce7" width="70%">
</p>

# Informe de la Regresión Lineal

## **Introducción**
El monoxido de carbono es un gas inodoro e incoloro que se produce  cuando los combustibles a  base de carbono  como la gasolina,gas natural y el quiroseno, no se queman completamente. Este gas puede causar  graves consecuencias en la salud humana y en el medio ambiente.
El presente informe  se centra en el analisis de los niveles  de monoxido de carbono en Nevada, Estados unidos,  durante los años 2022 y 2023. Se escogieron estos años ya que al ser los más recientes, la información nos ayuda a proyectar escenarios más adelantes. Nevada es conocido por sus amplios desiertos, centro turísticos y rápido cremiento demográfico.
Nuestro análisis se basa en datos recopilados que incluyen la concentración máxima diaria de CO en 8 horas, el Índice de Calidad del Aire (AQI) diario, y otros parámetros relacionados. Utilizamos métodos estadísticos, incluyendo análisis de correlación y regresión lineal, para examinar las relaciones entre estas variables y entender mejor los patrones de contaminación por CO en la región. Asi mismo, este    estudio es particularmente relevante debido a que se consideran los estándares nacionales de calidad del aire establecidos por la Agencia de Protección Ambiental (EPA) de los Estados Unidos, que fija límites de 9 partes por millón (ppm) para un promedio de 8 horas y 35 ppm para un promedio de 1 hora.
A través de este informe, buscamos proporcionar una visión detallada de la situación del monóxido de carbono en Nevada, identificar tendencias a lo largo del tiempo, y ofrecer insights que puedan ser útiles para la toma de decisiones en materia de calidad del aire,todo ello se muestra en las siguiente secciones.


## **Metodología**

Para el analísis de la concentración máxima diaria del CO en 8 horas y el AQI. Se tomaron en cuenta los valores minimos, maximos de cada uno así como su desviación estandar. Además de ello, se ha realizado regresión lineal en codigo python con el fin facilitarnos la comprensión de los datos orginiales. La regresión lineal es un método de análisis estadístico que busca modelar la relación entre una variable dependiente y una variable independiente. En nuestro caso, la variable dependiente es el indice de calidad del aire y la variable independiente es la concentración de monoxido de carbono. Así se obtuvieron la toma del coeficiente para la formulación de la ecuación de la recta y el valor de R cuadrado.

## **Resultados**
### Matriz de correlación y Heatmap en el 2022 y 2023

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Tabla%202022&2023.png?raw=true" alt="matriz de correlacion_tarea" width="140%">
</p>

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Heatmap%202022&2023.png?raw=true" width="70%">
</p>


Al comparar las siguientes correlaciones:

- Concentración máxima diaria de CO en 8 horas vs Indice de Calidad del Aire diario:
La correlación 0.998721 Lo que explica que existe una correlación positiva casi perfecta entre la concentración máxima diaria de CO en 8 horas y el valor diario de AQI (Índice de Calidad del Aire). Esto indica que a medida que aumenta la concentración de CO, el valor del AQI también aumenta casi de manera proporcional.

- Concentración máxima diaria de CO en 8 horas vs Observaciones diarias:
La correlación es 0.069491, positiva pero muy débil entre la concentración máxima diaria de CO en 8 horas y el conteo diario de observaciones. Esto sugiere que no hay una relación significativa entre estas variables.

- Indice de Calidad del Aire diario vs Observaciones diarias:
La correlación es 0.068541, similar a la relación anterior, la correlación entre el valor diario de AQI y el conteo diario de observaciones es muy débil, indicando poca o ninguna relación lineal.

### Gráfica de datos de frecuencia de la concentración máxima diaria de CO en 8 horas e Indice de Calidad del Aire diario

<p align="center">
<p float="left">  
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Freq%20CO%202022.png?raw=true" width="500" height="320" />  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Freq%20AQI%202022.png?raw=true" width="500" height="320" />  </p>

Tomando en cuenta como eje x concentración máxima diaria de CO en 8 horas y el eje y el Indice de Calidad del Aire diario, se realizo la regresión lineal y se obtuvieron los siguientes resultados.

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/RL%202022.png?raw=true" width="140%">
</p>

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Gr%C3%A1fica%202022.png?raw=true" width="140%">
</p>

### Matriz de correlación y Heatmap en el 2023 

<p align="center">
  <img src="https://github.com/user-attachments/assets/8ca33e8c-a1e5-42d3-aee8-2b2b55065740" alt="matriz de correlacion_tarea_2023" width="140%">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c766ac4-7782-47bf-95b4-39f3e3ad248b" alt="heatmap_tarea_2023" width="70%">
</p>


Análisis de la Matriz de Correlación 2023:

- Concentración máxima diaria de CO en 8 horas vs Indice de Calidad del Aire diario:
Correlación: 0.998755
Hay una correlación positiva casi perfecta entre la concentración máxima diaria de CO en 8 horas y el valor diario de AQI. Esto refuerza la idea de que el aumento en la concentración de CO está fuertemente asociado con un aumento en el valor del AQI.

- Concentración máxima diaria de CO en 8 horas vs Observaciones diarias:
Correlación: -0.017442
Existe una correlación negativa muy débil entre la concentración máxima diaria de CO en 8 horas y el conteo diario de observaciones. Esta relación es insignificante, lo que sugiere que estas dos variables no están linealmente relacionadas.

- Indice de Calidad del Aire diario vs Observaciones diarias:
Correlación: -0.017498
La relación entre el valor diario de AQI y el conteo diario de observaciones también es negativa y muy débil, indicando que no existe una relación significativa entre estas variables.

### Gráfica de datos de frecuencia de la concentración máxima diaria de CO en 8 horas e Indice de Calidad del Aire diario

<p align="center">
<p float="left">  
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Freq%20CO%202023.png?raw=true" width="500" height="320" />  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Freq%20AQI%202023.png?raw=true" width="500" height="320" />  </p>

Tomando en cuenta como eje x concentración máxima diaria de CO en 8 horas y el eje y el Indice de Calidad del Aire diario, se realizo la regresión lineal y se obtuvieron los siguientes resultados.

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/RL%202023.png?raw=true" width="140%">
</p>

<p align="center">
  <img src="https://github.com/JefHuiza/Proyectos_de_Ingenieria/blob/main/Entregables/Entregable_1/entregables/Gr%C3%A1fica%202023.png?raw=true" width="140%">
</p>

## **Discusión**
 El análisis comparativo de las correlaciones entre la concentración máxima diaria de CO en 8 horas, el Índice de Calidad del Aire (AQI) diario y el número de observaciones diarias para los años 2022 y 2023 revela varios hallazgos importantes. En ambos años, se observa una relación consistente entre el monóxido de carbono y la calidad del aire en Nevada. La correlación casi perfecta entre la concentración de CO y el AQI sugiere que el control de las emisiones de CO debería ser una prioridad en las políticas ambientales para mejorar la calidad del aire. Por otro lado, las correlaciones débiles con el número de observaciones diarias indican que factores externos o el propio método de recolección de datos pueden estar influyendo en la falta de una relación significativa entre el AQI y la concentración de CO. Además, de acuerdo al cuadro de frecuencias, se observa que las concentraciones de monóxido de carbono en 8 horas en 2022 son ligeramente superiores a las de 2023 aunque la concentración se mantuvo relativamente constante en ambos años.



## **Referencias**

[^1]: Raub, J. A., & Benignus, V. A. (2002). Carbon monoxide and the nervous system. Neuroscience & Biobehavioral Reviews, 26(8), 925-940.

[^2]: Agencia de Protección Ambiental de los Estados Unidos, "National Ambient Air Quality Standards (NAAQS) for Carbon Monoxide," EPA, 2023. [Online]. Available: https://www.epa.gov/co-pollution. [Accessed: 23-Aug-2024].
