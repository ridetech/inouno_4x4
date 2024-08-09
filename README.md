# inouno_4x4
Arduino uno 4in digitales x 4out de salida en relay shield. contiene webserver para manejar el tiempo de disparo entre la activacion de los input digitales y el disparo de los relay

Programacion para ARDUINO UNO.

Tomamos 4 entradas digitales, las cuales hacen referencia a 4 salidas.

common GND (siguiente a pin d13 anterior a AREF) <br>
Entrada 1 (output pin 4)  ---> pin8 <br>
Entrada 2 (output pin 5)  ---> pin9 <br>
Entrada 3 (output pin 6)  ---> pin10 <br>
Entrada 4 (output pin 7)  ---> pin11 <br>

Salidas relacionadas con el Shield de relays <br>

Salida 1 ---> pin 4 <br>
Salida 2 ---> pin 5 <br>
Salida 3 ---> pin 6 <br>
Salida 4 ---> pin 7 <br>

Se configuro en el codigo un test inicial de todos los relay (del 1 al 4 en secuencia) con lo que al encender, cambiara de estado iniciando por relay1, en 2 segundos relay2 y asi consecutivamente hasta el 4. Una vez terminado el test, se regresan todos los relay,s a la normal.

El proyecto contiene un servidor web protegido por usuario y password con el que es posible de manera remota cambiar los umbrales de disparo almacenados.

A fin de no registrar de manera erronea los estados, se habilito la resistencia pullup interna
