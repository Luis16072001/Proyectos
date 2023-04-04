# README Macro Valuación de Derivados a tiempo discreto mediente Árboles Multiplicativos

## Contenido

La macro está diseñada para calcular el valor de un derivado a lo largo del tiempo, teniendo en cuenta la posibilidad de que el derivado no pague dividendos o pague dividendos ya sean discretos o continuos. Dichos cálculos estarán disponibles para los siguientes derivados:

  1. Call Europeo sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  2. Put Europeo sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  3. Call Digital sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  4. Put Digital sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  5. Call Americano sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  6. Put Americano sin pago de dividendos, con pago de dividendos continuos y con pago de dividendos discretos.
  7. Call Asiático sin pago de dividendos y con pago de dividendos continuos.
  8. Put Asiático sin pago de dividendos y con pago de dividendos continuos.

Las salidas resultantes de los cálculos son las siguientes:

  1. El factor u mediante el cual el activo subyacente aumenta su precio.
  2. El factor d mediante el cual el activo subyacente disminuye su precio.
  3. La probabilidad q asociada a la medida de riesgo neutral Q.
  4. El factor de descuento asociado a la cuenta de mercado de dinero B.
  5. El factor de acumulación asociado a la cuenta de mercado de dinero B^-1.
  6. Para los derivados que pagan dividendos continuos, el factor de acumulación asociado a los cupones B_E.
  7. Para los derivados que pagan dividendos continuos, el factor de descuento asociado a los cupones B_E.
  8. El valor de Delta que indica el espaciado entre cada uno de los periodos del árbol.
  9. El precio Forward/Valor del derivado al día de hoy.
  10. Árbol de los precios del subyacente.
  11. Árbol con el valor del derivado a lo largo del tiempo.
  12. Árbol con la cantidad de activo subyacente necesaria en cada periodo de tiempo para llevar a cabo la estrategia de cobertura.
  13. Árbol con la cantidad de dinero en la cuenta de mercado de dinero que se debe tener en cada periodo de tiempo para llevar a cabo la estrategia de cobertura.

## Funcionamiento

### Ingreso de datos

Todos los datos deberán ser ingresados en la hoja "Datos".

  1. Seleccione en el recuadro "Selecciona Dividendos" el tipo de dividendos que va a pagar el derivado que se desea valuar. En caso de que no pague dividendos seleccionar la opción "Sin dividendos"
  2. Seleccione en el recuadro "Selecciona el Derivado" el derivado que desea valuar.
  3. En el apartado de "Ingresa tus datos", debera proporcionar los parametros necesarios para poder llevar a cabo dicha valuación en su correspondiente celda.
     a) Volatilidad asociada al derivado
     b) Tasa asociada a la cuenta de mercado de dinero, debe ser una tasa efectiva continua de periodicidad anual
     c) El número de periodos a considerar en el árbol. En el caso de los derivados Asiáticos el límite de periodos es de 10, para el resto de derivados no hay límite.
     d) Vencimiento del derivado en años.
     d) Precio del subyacente al día de hoy
     c) Precio strike pactado
     e) En el caso de los Derivados que pagan dividendos, se debe incluir la "Tasa Extranjera" correspondiente a dichos cupones
     f) Para el caso de los derivados digitales, se deberá agregar el parámetro "M" el cual indica la barrera asociada.
     g) Para el caso de los derivados que pagan dividendos discretos, se deberá proporcionar el VP de los dividendos.

### Cálculos y salidas

  4. Una vez ingresados los datos del punto anterior, se podrá realizar todos los cálculos mencionados anteriormente dando clic en el botón "Calcular Árboles". En caso de que el cálculo no se encuentre disponible, se indicará mediante una nota de color rojo debajo de dicho botón.

  5. Si el derivado es de tipo Asiático, antes de realizar los cálculos se deberán calcular las trayectorias dando clic en el botón "Trayectorias". En caso de ser necesario se indicará en color rojo arriba de dicho botón.

  6. De las salidas 1 a 9, mencionadas anteriormente, se mostrarán en la hoja de "Datos" en el apartado de "Salidas". Los precios del subyacente se mostrarán en la hoja de "Subyacente". El valor del derivado se mostrará en la hoja "Derivado". La cantidad de activo subyacente necesaria para el portafolio de cobertura se mostrará en la hoja "Alpha". La cantidad de dinero en la cuenta de mercado de dinero necesaria para el portafolio de cobertura se mostrará en la hoja "Beta". La hoja "Auxiliar" se debe ignorar, solo se usa para cálculos auxiliares.

