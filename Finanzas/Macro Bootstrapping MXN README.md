# Bootstrapping de MXN para IRS

Este proyecto se desarrolló una macro diseñada para realizar un Bootstrapping de MXN bajo los métodos de interpolación lineal e interpolación en tasas continuas. Esto permite que, dadas las tasas nx1 (Tasas Par Swap) de mercado, se puedan calcular las tasas Par Swap para los periodos intermedios en los cuales no se conoce como dicha tasa. Esto nos permite calcular los factores de descuento P(0,j28) con j = 1,2,3,4,...,130, que resultan de gran utilidad para el cálculo del precio de ciertos instrumentos financieros en los que estos factores estén involucrados, como FRA, IRS, Swaptions, entre otros.

Nota. nx1 indica que se van a realizar n intercambios de tasa fija contra 1 intercambio de TIIE 28, donde n = 1, 3, 6, 9, 13, 26, 39, 52, 65, 91, 130.

## Funcionamiento

### Ingreso de datos

Los datos debrán ser ingresados en los recuadros correspondientes de la hoja "Datos". Dichos datos a ingresar son los siguientes:

1. Vector de tasas. Se debe proporcionar el valor de la TIIE de fondeo, la TIIE 28 (el equivalente a un 1x1), y las tasas nx1 para n = 3, 6, 9, 13, 26, 39, 52, 65, 91, 130.
2. Se debe establecer una Fecha de Valuación. Por defecto se encuentra la fecha del día de hoy, sin embargo, puede ser modificada a cualquier otra fecha de acuerdo a las necesidades.
3. Seleccionar el tipo de Bootstrapping. Se cuenta con un Bootstrapping por interpolación lineal y otro por interpolación de tasas continuas.
4. Elegir la convención de año calendario. Se cuenta con las convenciones de 360 y 365.
5. Elegir la convención para los Day Count Fraction. Se cuenta con las convenciones de Día hábil siguiente y Día hábil anterior. Además, por defecto ya se cuenta con un vector de holidays aplicado sobre estas convenciones.

Una vez ingresados todos los datos anteriores, para realizar los cálculos se deberá dar clic en el botón "Bootstrapping".

### Salidas

Las salidas se mostrarán en la hoja de Bootstrapping, y son las siguientes:

1. Fechas de Fixing.
2. Fechas de Inicio.
3. Fechas de Fin.
4. Fecha de pago (Payment Day).
5. Factores de descuento.

Estas salidas corresponden a cada una de las tasas nx1, con n = 1, 2, 3,...,130.
