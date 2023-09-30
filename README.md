# Robotica_lab2

Para este laboratorio se tomó como base el trabajo realizado en el Laboratorio 1, donde el robot se programó para escribir las iniciales de cada integrante del equipo. En este caso, nos limitamos a escribir unicamente la primera palabra ("JAIME").

Partiendo de esta base se incorporó una
nueva funcionalidad pues ahora el problema nos exige la utilización del tablero de usuario y para ello se requiere la definición de entradas y salidas digitales en nuestro programa.
Como primer punto, se agregaron dos entradas y dos salidas digitales en nuestro programa de roboStudio. 
Tabla de entradas y salidas digitales:

[![IMG-20230930-WA0042.jpg](https://i.postimg.cc/YqVVFfB7/IMG-20230930-WA0042.jpg)](https://postimg.cc/56BndztK)


La siguiente imagen muestra el tablero, donde los botones verdes corresponden a las entradas, también se muestran los LEDs correspondientes a las salidas.

[![IMG-20230930-145043.jpg](https://i.postimg.cc/mk9ZsZQ1/IMG-20230930-145043.jpg)](https://postimg.cc/p52MQHcP)

Una vez establecidas las entradas y salidas, se procedió a modificar el código, para ello se agregaron dos condicionales dentro de un ciclo WHILE. La primera condicional establece que, cuando se pulse el botón 1, el led 1 se enciende y el robot realizará la escritura corrspondiente, una vez escrita la palabra, el robot regresa a la posición inicial y el led 1 se apaga.

La segunda condicional establece que, cuando se presionesione el segundo botón, el robot se va a la posición de mantenimiento, una vez llegada a esta posición, el led 2 se apaga.
La siguiente imagen nos muestra el bucle y las condicionales:

[![IMG-20230930-164930.jpg](https://i.postimg.cc/cJcsx5gT/IMG-20230930-164930.jpg)](https://postimg.cc/R3NrGdTn)