# PI-02-DS04
Proyecto Nº 2 - Cohorte 4
### RESUMEN DEL CASO

Entendemos que asignar o catalogar una clasidicador a la compra de un inmueble según el monto promedio de la transacción depende en mayor medida del Valor Comercial, como del valor de la infraestructura.

Asimismo, se percibe que las propiedades no son baratas ni caras según el vendedor u ofertante, sino que este indicador se configura cuanto se realiza la operación y depende
del valor que se paga y del tiempo en que se tarda en concretar una venta.

De maneea que:
La propiedad puede ser barata, según el vendedor, pero en tanto no se venda y se pague el precio solicitado podría pensarse que su valor es elevado.

Por ello, se ha creado un indicador adicional: days_to_sale calculado como la diferencia entre las fechas en que se oferto el bien y la fecha en que se realizó la venta.
Mientras más demoró en venderse una propiedad podríamos suponer que no es tan barata.
El coeficiente de correlación sustenta bien esta hipótesis.

## ANLÁLISIS EXPLORATORIO DE DATOS
Prima la tarea de identificar de la estructura de los datos cuáles podrían ser determinantes en el pronóstico de clasificación.
Asimismo, y desde el punto de vista técnico es conveniente identificar datos categóricos y numéricos, asi como si habrá que transformar los datos cualitativos en ordinales
o en nominales.

Esta información puede ir encausando el trabajo y permite oragnizar y priorizar las tareas.

En ese sentido, se trabajó en la pronta depuración de columnas innecesarias a fin de hacer el trabajo más ágil, ya que la demanda de recursos (espacio y memoria) son
altos.

#Eliminación de Columnas:
Son evidentemente innecesarios, campos como "país", "moneda", etc..., cuando son los únicos entre miles.
  

Con ayuda de df.describe() y df.describe(inlcude=object) se puede identificar visualmente qué columnas presentan altísima frecuencia en relación al total de filas.

![This is an image](https://github.com/Duilius/PI-02-DS04/blob/main/frecuencia.jpg)


