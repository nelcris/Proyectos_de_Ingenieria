<p align="center">
  <img src="https://github.com/JefHuiza/Fundamentos-de-Dise-o/assets/156036185/d3c66dfb-5faa-419b-bf1b-d897ea110ce7" width="70%">
</p>

# Informe de la Regresión Lineal

## **Introducción**
El monoxido de carbono es un gas inodoro e incoloro que se produce  cuando los combustibles a  base de carbono  como la gasolina,gas natural y el quiroseno, no se queman completamente. Este gas puede causar  graves consecuencias en la salud humana y en el medio ambiente.
El presente informe  se centra en el analisis de los niveles  de monoxido de carbono en Nevada, Estados unidos,  durante los años 2022 y 2023. Nevada es conocido por sus amplios desiertos, centro turísticos y rápido cremiento demográfico, ..
El objetivo de este  estudio es examinar las tendencias 



## **Metodología**
  (Métodos utilizados)
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


Medir la concentración de monóxido de carbono (CO) en los Estados Unidos es crucial para proteger la salud pública y el medio ambiente . En cuanto a los valores de CO permitidos, la Agencia de Protección Ambiental (EPA) establece un estándar nacional de calidad del aire para CO de 9 partes por millón (ppm) sobre un promedio de 8 horas y 35 ppm sobre un promedio de 1 hora [^2].
Ahora bien, estos datos que se tiene son datos exteriores, que nos indica los niveles donde el CO ya literalmente es menos la concentracion; en cambio estos datos no son  datos interiores, el monitoreo de CO en interiores no es responsabilidad de la EPA, ya que el CO en interiores generalmente proviene de fuentes como calentadores de gas, estufas, chimeneas, generadores portátiles y vehículos que funcionan en espacios cerrados. Para la detección de CO en interiores, se recomienda a los propietarios de viviendas y edificios el uso de detectores de monóxido de carbono para prevenir intoxicaciones. Los niveles en las casas promedio sin estufas de gas varían de 0,5 a 5 partes por millón (ppm). Los niveles cercanos a las estufas de gas ajustados correctamente suelen ser de 5 a 15 ppm y aquellos cerca de estufas poco ajustadas pueden ser de 30 ppm o más. Esta informacion nos sirve para hacer un contraste claro de que los interiores son por mucho en ocasiones mayoes que los estandares dicho por el EPA.

El monóxido de carbono (CO) en la atmósfera es generalmente considerado perjudicial. A diferencia del dióxido de carbono (CO₂), que es esencial para la fotosíntesis y tiene un papel en el ciclo de vida de las plantas, el CO es un contaminante tóxico para los seres humanos y animales. Se une a la hemoglobina en la sangre, impidiendo que el oxígeno se transporte adecuadamente por el cuerpo, lo que puede llevar a la asfixia y, en altas concentraciones, a la muerte [^1]. El CO se produce principalmente por la combustión incompleta de combustibles fósiles, como en los motores de los vehículos y las estufas mal ventiladas.

De acuerdo a la regresión lineal realizada, las relaciones de variables más destacadas son las correlaciones casi perfectas entre la concentración máxima diaria de CO en 8 horas y el valor de AQI, así como entre el porcentaje de datos completos y el conteo diario de observaciones. Al comparar los datos de ambos años, los patrones de correlación se mantienen en gran medida similares. Por lo que la relación entre estas variables se considera directa y exacta.


## **Referencias** _(en formato IEEE)_

[^1]: Raub, J. A., & Benignus, V. A. (2002). Carbon monoxide and the nervous system. Neuroscience & Biobehavioral Reviews, 26(8), 925-940.

[^2]: Agencia de Protección Ambiental de los Estados Unidos, "National Ambient Air Quality Standards (NAAQS) for Carbon Monoxide," EPA, 2023. [Online]. Available: https://www.epa.gov/co-pollution. [Accessed: 23-Aug-2024].
“Impacto del monóxido de carbono en la calidad del aire de los interiores | US EPA”. US EPA. Accedido el 24 de agosto de 2024. [En línea]. Disponible: https://espanol.epa.gov/cai/impacto-del-monoxido-de-carbono-en-la-calidad-del-aire-de-los-interiores

