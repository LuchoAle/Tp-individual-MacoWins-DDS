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

![Diagrama de clases](https://user-images.githubusercontent.com/102762669/231598987-8ac8a61d-f0c7-4731-ba62-fee0fbbc85ca.jpg)

- Pseudocodigo:

![image](https://user-images.githubusercontent.com/102762669/231605230-aef85c39-9a9d-4bcb-8ed9-72aa11db3173.png)

![image](https://user-images.githubusercontent.com/102762669/231605289-31f12ff9-09c8-4f3a-96ec-8eda18c7a448.png)


3) Explicar todo lo que se considere necesario en prosa

La clase registro tiene cargado en una lista todas las ventas y es la que se encarga de obtener la ganancia del dia en base a una fecha.

4) SI SE DESCARTA ALGUNA ALTERNATIVA DURANTE EL DESARROLLO DE LA SOLUCIÓN, O SI SE TIENE OTRA SOLUCIÓN, EXPLICARLA BREVEMENTE

- Tenia pensado que existieran distintos registros para cada dia con las ventas de ese dia cargados en la clase. Pero si existiera una base de datos sería mejor cargar las ventas en base a los dias pedidos por una clase registro general.


