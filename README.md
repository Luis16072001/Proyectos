# Proyectos de R y VBA
Este repositorio contiene algunos de los proyectos más importantes que he realizado en R y en VBA. A continuación, se describen brevemente los proyectos 
en R:

## Proyectos en R
### Autor: 
- Luis Alberto Cruz Barrios
### Selección de variables mediante aprendizaje no supervisado
En este proyecto se utilizó un algoritmo de aprendizaje no supervisado para la selección de variables, con el objetivo de identificar las variables más 
importantes en un modelo estadístico. El proyecto incluye un reporte detallado de los resultados obtenidos y el código implementado para llegar a ellos.

Para llevar a cabo este proyecto, se utilizó un conjunto de datos y se aplicaron diferentes métodos de selección de variables basados en los criterios de 
información AIC y BIC. En el reporte se muestra cómo los diferentes métodos de selección de variables afectan al modelo estadístico resultante y se comparan 
los resultados de cada método. Además, se presenta el código utilizado para la implementación de los diferentes métodos de selección de variables.

### Prediccion con Variables Continuas mediante aprendizaje no supervisado
En este proyecto se implementó un algoritmo de aprendizaje no supervisado para la selección de las variables continuas que formarán el modelo con mejor poder 
predictivo. Se incluye un reporte detallado de los resultados, en el que se muestra el desempeño del modelo y se comparan diferentes métodos de selección de 
variables. Además, se presenta el código implementado para llegar a los resultados.

Para llevar a cabo este proyecto, se utilizó un conjunto de datos con variables continuas y se aplicó un algoritmo de aprendizaje no supervisado para 
identificar las variables más relevantes para el modelo predictivo. El reporte incluye gráficos y estadísticas para mostrar cómo el modelo seleccionado tiene 
un mejor desempeño que otros modelos basados en diferentes métodos de selección de variables.

En la sección de código, se puede encontrar el código completo utilizado para la implementación del algoritmo de selección de variables, así como para la 
creación del modelo predictivo. Además, se incluyen comentarios explicando cada paso del proceso.

## Proyectos en Visual Basic
### Autores: 
- Montserrat Fernández Neria
- Luis Alberto Cruz Barrios
### Valuación de derivados a tiempo discreto mediante Árboles Multiplicativos

En este proyecto se desarrolló una macro en VBA para valuar diferentes tipos de derivados mediante Árboles Multiplicativos. La macro también permite generar 
un portafolio de cobertura para el derivado seleccionado, considerando pagos de dividendos discretos o continuos.

La macro genera 4 salidas: árbol de precios, árbol del valor del derivado, árbol de la cantidad de subyacente y árbol de la cantidad de la cuenta de mercado 
de dinero. En el README correspondiente a este proyecto, se incluyen todos los detalles sobre el uso de la macro, los parámetros que se deben ingresar y los 
cálculos que se pueden realizar para valorar y cubrir el derivado seleccionado.

### Bootstrapping de MXN para IRS

En este proyecto se desarrolló un Bootstrapping mediante el cual, dadas las tasas nx1 (Tasas Par swap) de mercado, se calculan las tasas Par Swap para los 
periodos intermedios en los cuales no se conoce dicha tasa. Se utilizaron diferentes métodos de interpolación para este cálculo. Una vez obtenidas las tasas 
Par Swap para todos los periodos, se calcularon los factores de descuento ($P(0,j28),j=1,2,3,4...$), los cuales resultan útiles para el cálculo del precio de 
ciertos instrumentos financieros en los que estos factores estén involucrados, como FRA, IRS, Swaptions, entre otros.

En el README correspondiente a este proyecto se pueden encontrar todos los detalles sobre el proceso de Bootstrapping, los métodos de interpolación 
utilizados y cómo se calculan los factores de descuento.
