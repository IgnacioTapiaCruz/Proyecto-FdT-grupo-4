Actualmente, Chile y el mundo se enfrentan a la crisis climática. El calentamiento global ha aumentado con el incremento de las emisiones de gases de efecto invernadero (GEI), siendo el más significativo el dióxido de carbono (CO2). Una de las principales fuentes de emisión de este gas es la quema de combustibles fósiles para la generación de energía, que en Chile para el año 2020 representó el 75% de las emisiones de CO2. La liberación de estos gases a la atmósfera induce el calentamiento de los océanos y del aire cercano a la superficie terrestre, lo que impacta negativamente en ecosistemas completos, alterando su flora y fauna. 

Es por esto que en los últimos años se ha buscado la diversificación del suministro eléctrico por medio de tecnologías renovables y bajas en emisiones de carbono. Una de las alternativas es la energía solar térmica, la cual cuenta con bajas emisiones de dióxido de carbono y en Chile tiene gran potencial en la zona norte del país, debido a que agrupa condiciones favorables como clima extremadamente seco, bajas precipitaciones y altas temperaturas. Es importante agregar que dado a la dependencia de la disponibilidad de luz solar, es necesario acumular la energía en un sistema de almacenamiento térmico, de modo que se puedan dejar  de lado los combustibles fósiles asegurando la estabilidad y continuidad en la distribución de energía, además de satisfacer la demanda. 

Para ello, se estudiará un tanque de almacenamiento térmico de una planta termosolar, con el fin de comprender los fenómenos de transporte que involucra, analizar su eficacia y proponer mejoras de ser necesario, de modo que posteriormente se pueda promover el uso de energía termosolar como sustituto a los combustibles fósiles.

El sistema estudiado es un tanque cilíndrico de medidas específicas, que posee una capa aislante en su exterior. En el interior del tanque se encuentra una mezcla de sales fundidas a alta temperatura, para el caso estudiado la mezcla está compuesta específicamente de 60% NaNO3 + 40% KNO3 debido a la utilidad industrial. 


Descripción del método
numérico utilizado
(30%)

Para la resolución de las ecuaciones de los distintos perfiles modelados se utilizó el método de sobrerrelajación sucesiva (SOR) aplicable a las ecuaciones diferenciales elípticas del sistema. Además, este método permite resolver dichas ecuaciones en un dominio bidimensional, tras la generación de una grilla computacional para una cantidad específica de nodos en el eje radial y axial. 

Para esto, se cumple con un esquema de discretización basado en diferencias finitas, específico para cada ecuación gobernante y sus respectivas condiciones de borde, presentado a continuación. Las ecuaciones y sus condiciones de borde discretizadas se encuentran en el Jupyter Notebook se la solución.

- Perfil de velocidad: a través de diferencias hacia delante de primer orden (primeras derivadas) y diferencias centrales de segundo orden (segundas derivadas).
- Perfil de temperatura interior: a través de diferencias hacia delante de primer orden (primeras derivadas) y diferencias centrales de segundo orden (segundas derivadas).
- Perfil de temperatura en aislante: a través de diferencias finitas centrales de segundo orden.
- Para las condiciones de borde se usaron aproximaciones hacia adelante y hacia atrás, dependiendo de la condición para la resolución de los distintos perfiles.

Para ejecutar correctamente el código, basta con descargar el archivo con la solución y abrirlo en alguna consola para pyhton o en la nube (Google Colab), para ir ejecutando las celdas de arriba hacia abajo. Así aparecerán los distintos resultados con sus gráficos correspondientes, a medida que se vaya ejecutando las celdas.

Gráfico 1: Perfil de velocidad en pared aislada.
![Imagen de WhatsApp 2025-12-09 a las 11 30 05_b82a6e90](https://github.com/user-attachments/assets/4766699c-a13c-43b1-af08-f30ab72a0ec6)

