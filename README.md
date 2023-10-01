# Robotica_lab2
## Integrantes

- Norma Lorena Martinez Zavala
- Miguel Angel Sarmiento Cabarcas
- Jaime Andres Sanchez Peralta

## Descripción de solución.
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


## Diagrama de flujo

[![IMG-20230930-WA0044.jpg](https://i.postimg.cc/Pxx9Z6Jt/IMG-20230930-WA0044.jpg)](https://postimg.cc/06TV1073)


## Descripción de las funciones utilizadas

Para este laboratorio se usaron nuevas funciones en el código, las cuáles son descritas a continución:
 
-set: Esta función se usa para establecer variables, en este caso definimos "out1" y "out2".

-WHILE TRUE DO: Inicia el bucle infinito, lo que significa que el código dentro de este bucle se ejecutará repetidamente sin fin.

-IF y ELSEIF: Son los condicionales con los que se ejecutará el código.

-!SetDO: Este comando establece el estado dea salida digital, configuarmos para Out1 en 0 (apagado).

-reset: Se utiliza para reestablecer variables


-TPWrite: Utilizado para la impresión de mensajes

En cuanto a los procedimiendos "Path_80" y "Path_90", se utilizó la función -->MoveAbsJ<-- la cual indica que se está realizando un movimiento de tipo absoluto para alcanzar una posición específica, la cual es: -->JointTarget_2<--, finalmente, se específican los parámetros de velocidad, la herramienta y el objeto de trabajo.
