# vuebots | OBJETIVO 

Desarrollar una interfaz con VueJs que permita correr una carrera de bots visible sobre un mapa de Google Maps.

La competencia consiste en que el usuario indica un punto sobre el mapa al que todos los bots deben acercarse en línea recta cambiando su posición cada 1 segundo. Los bots se encuentran ubicados de manera aleatoria en la ciudad donde vives.

Debes cumplir con cada uno de los siguientes puntos:

La interfaz debe mostrar un mapa de Google Maps y un recuadro donde se listan los bots. El número inicial de bots que empiezan en la competencia debe ser un número aleatorio entre 5 y 10.

1. Los bots se mueven en dirección al punto marcado por el usuario como meta. Cada bot solo puede hacer un movimiento cada 1 segundo de una distancia aleatoria entre 50 y 100 metros.


2. Cada bot tiene una batería que dura 100 unidades, y cada cambio de posición gasta un número aleatorio entre 10 y 30 unidades.


3. Cuando un bot quede sin batería debe detenerse por 6 segundos para volver a empezar con 100 unidades.


4. Se debe mostrar un botón “Agregar nuevo Bot”, que al presionarse incrementa en 1 el número de bots en competencia. Al agregarse, se ubica de manera aleatoria en la ciudad y de inmediato inicia su trayecto a la meta


5. La interfaz debe mostrar de manera fácil el estado de toda la competencia, estado de los bots, posición de cada uno, distancia hacia la meta y todo lo que considere útil para el usuario


6. El bot que esté más cerca a la meta debe mostrarse con color verde. El último con color rojo, y el resto con color amarillo.


7. Alojar la prueba en algún servicio de tal manera que nos puedas enviar la url para nosotros visualizarlo en funcionamiento.