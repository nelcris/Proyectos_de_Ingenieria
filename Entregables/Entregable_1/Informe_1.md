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
### Matriz de correlación y Heatmap (2022)

<p align="center">
  <img src="https://github.com/user-attachments/assets/33620491-bfb0-44e1-a29b-2cf45f355c01" alt="matriz de correlacion_tarea" width="140%">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a47653d3-2e7f-46b7-bc0e-5683a5b7e036" alt="heatmap_Tarea" width="70%">
</p>


Al comparar las siguientes correlaciones:


- Daily Max 8-hour CO Concentration vs Daily AQI Value la correlación es 0.998721 Lo que explica que existe una correlación positiva casi perfecta entre la concentración máxima diaria de CO en 8 horas y el valor diario de AQI (Índice de Calidad del Aire). Esto indica que a medida que aumenta la concentración de CO, el valor del AQI también aumenta casi de manera proporcional.
Daily Max 8-hour CO Concentration vs Daily Obs Count:
La correlación es 0.069491, positiva pero muy débil entre la concentración máxima diaria de CO en 8 horas y el conteo diario de observaciones. Esto sugiere que no hay una relación significativa entre estas variables.

- Daily AQI Value vs Daily Obs Count:
La correlación es 0.068541, similar a la relación anterior, la correlación entre el valor diario de AQI y el conteo diario de observaciones es muy débil, indicando poca o ninguna relación lineal.

- Percent Complete vs AQS Parameter Code:
La correlación es 0.068797. La relación entre el porcentaje de datos completos y el código de parámetros AQS también es muy débil, lo que indica una relación insignificante entre estas variables.

- Percent Complete vs Daily Obs Count:
La correlación es 0.999971. Existe una correlación positiva casi perfecta entre el porcentaje de datos completos y el conteo diario de observaciones. Esto sugiere que cuando hay un mayor porcentaje de datos completos, el número de observaciones diarias tiende a ser alto.

### Matriz de correlación y Heatmap (2023)

<p align="center">
  <img src="https://github.com/user-attachments/assets/8ca33e8c-a1e5-42d3-aee8-2b2b55065740" alt="matriz de correlacion_tarea_2023" width="140%">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c766ac4-7782-47bf-95b4-39f3e3ad248b" alt="heatmap_tarea_2023" width="70%">
</p>


Análisis de la Matriz de Correlación 2023:


- Daily Max 8-hour CO Concentration vs Daily AQI Value:
Correlación: 0.998755
Hay una correlación positiva casi perfecta entre la concentración máxima diaria de CO en 8 horas y el valor diario de AQI. Esto refuerza la idea de que el aumento en la concentración de CO está fuertemente asociado con un aumento en el valor del AQI.

- Daily Max 8-hour CO Concentration vs Daily Obs Count:
Correlación: -0.017442
Existe una correlación negativa muy débil entre la concentración máxima diaria de CO en 8 horas y el conteo diario de observaciones. Esta relación es insignificante, lo que sugiere que estas dos variables no están linealmente relacionadas.

- Daily AQI Value vs Daily Obs Count:
Correlación: -0.017498
La relación entre el valor diario de AQI y el conteo diario de observaciones también es negativa y muy débil, indicando que no existe una relación significativa entre estas variables.

- Percent Complete vs Daily Obs Count:
Correlación: 0.999975
La correlación positiva casi perfecta entre el porcentaje de datos completos y el conteo diario de observaciones indica una fuerte relación directa.

- Percent Complete vs AQS Parameter Code:
Correlación: -0.018200
La correlación entre el porcentaje de datos completos y el código de parámetros AQS sigue siendo muy débil y negativa, lo que indica poca o ninguna relación entre estas variables.

## **Discusión** _(opcional)_


El monóxido de carbono (CO) en la atmósfera es generalmente considerado perjudicial. A diferencia del dióxido de carbono (CO₂), que es esencial para la fotosíntesis y tiene un papel en el ciclo de vida de las plantas, el CO es un contaminante tóxico para los seres humanos y animales. Se une a la hemoglobina en la sangre, impidiendo que el oxígeno se transporte adecuadamente por el cuerpo, lo que puede llevar a la asfixia y, en altas concentraciones, a la muerte [^1]. El CO se produce principalmente por la combustión incompleta de combustibles fósiles, como en los motores de los vehículos y las estufas mal ventiladas.

Medir la concentración de monóxido de carbono (CO) en los Estados Unidos es crucial para proteger la salud pública y el medio ambiente . En cuanto a los valores de CO permitidos, la Agencia de Protección Ambiental (EPA) establece un estándar nacional de calidad del aire para CO de 9 partes por millón (ppm) sobre un promedio de 8 horas y 35 ppm sobre un promedio de 1 hora [^2].

De acuerdo a la regresión lineal realizada, las relaciones de variables más destacadas son las correlaciones casi perfectas entre la concentración máxima diaria de CO en 8 horas y el valor de AQI, así como entre el porcentaje de datos completos y el conteo diario de observaciones. Al comparar los datos de ambos años, los patrones de correlación se mantienen en gran medida similares. Por lo que la relación entre estas variables se considera directa y exacta.


## **Referencias** _(en formato IEEE)_

[^1]: Raub, J. A., & Benignus, V. A. (2002). Carbon monoxide and the nervous system. Neuroscience & Biobehavioral Reviews, 26(8), 925-940.

[^2]: Agencia de Protección Ambiental de los Estados Unidos, "National Ambient Air Quality Standards (NAAQS) for Carbon Monoxide," EPA, 2023. [Online]. Available: https://www.epa.gov/co-pollution. [Accessed: 23-Aug-2024].
