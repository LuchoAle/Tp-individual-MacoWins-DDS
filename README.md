# Tp-individual-MacoWins-DDS

1) Identificar los requerimientos:

Los requerimientos son las necesidades que tiene el usuario y se tienen que  ver plasmadas en el sistema solucion a implementar. Estos pueden ser requerimientos funcionales o no funcionales.

Requerimientos funcionales:

- Obtener precio venta de un prenda
- Obtener tipo de prenda 
- Calcular precio de venta
- Si la prenda tiene estado nuevo no modificar precio
- Si la prenda tiene estado promoción: Restar valor fijo definido por el usuario
- Si la prenda tiene estado liquidación: Es un 50% del valor del producto
- Registrar venta
- Obtener ganacias de un determinado día
- Realizar ventas en efectivo o tarjeta
- Permitir aplicar cuotas en caso de tarjeta, y generar el precio final

Requerimientos no funcionales: No se especifican

2) Presentar una solución usando el paradigma de objetos (pseudocódigo, diagrama de clases)

- Diagrama de clases: 

![Moc wins diagrama 2](https://user-images.githubusercontent.com/102762669/231790515-f6658b59-2508-4a49-900e-03dc6c36edfa.jpg)

- Pseudocodigo:

![image](https://user-images.githubusercontent.com/102762669/231791007-3ac653a1-1e8e-4bf8-b661-350ed2ca7df0.png)

![image](https://user-images.githubusercontent.com/102762669/231791069-42b8b1ea-ee29-42f2-8634-3cdeee091278.png)


3) Explicar todo lo que se considere necesario en prosa

La clase registro tiene cargado en una lista todas las ventas y es la que se encarga de obtener la ganancia del dia en base a una fecha.

Respecto a la interfaz estado y los estados: promocion y liquidacion, me di cuenta que realizan exactamente el mismo calculo pero con diferentes valores, es por eso que para ahorrar codigo decidi que liquidacion herede de promocion y solo se cambie el valor del atributo descuento.

4) SI SE DESCARTA ALGUNA ALTERNATIVA DURANTE EL DESARROLLO DE LA SOLUCIÓN, O SI SE TIENE OTRA SOLUCIÓN, EXPLICARLA BREVEMENTE

- Tenia pensado que existieran distintos registros para cada dia con las ventas de ese dia cargados en la clase. Pero si existiera una base de datos sería mejor cargar las ventas en base a los dias pedidos por una clase registro general.

- Otra alternativa descartada: 

![Diagrama de clases](https://user-images.githubusercontent.com/102762669/231598987-8ac8a61d-f0c7-4731-ba62-fee0fbbc85ca.jpg)

La siguiente fue descartada debido a que solo se podian registrar ventas de un mismo tipo de prenda por lo que si el usuario queria realizar otra compra de otra prende se tendría que realizar una venta distinta y esto implica volver a cargar datos.
