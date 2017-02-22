# Práctica 1 😉 #

## Modos de conexión a la Raspberry Pi 3 😀 ##

### 1.- Vía HDMI ###

Solo hay que conectar un monitor por el puerto **HDMI** y un teclado para poder ejecutar comandos en shell, opcionalmente podemos conectar un mouse para usar las aplicaciones mediante interfaz gráfica.

![RaspberryHDMI](https://raw.githubusercontent.com/LuisEGR/embebidos-17-2/788d264a0adef514dda11da6d7e1153b7ec77506/practicas/practica1/LuisEGR/img/via_hdmi.jpg "LRaspberry Pi HDMI")

### 2.- Vía SSH ###

Para **SSH** hay que tener conexión con la Raspberry Pi, en nuestro caso usamos una red local, una vez que encontramos la dirección ip de nuestra tarjeta, solo ejecutamos el comando:
```shell
ssh pi@192.168.43.220
```

en donde **192.168.43.220** corresponde a la ip de la Raspberry Pi, luego de eso se nos solicita la contraseña y por defecto, si no se ha modificado, es **raspberry**.

![RaspberryHDMI](https://raw.githubusercontent.com/LuisEGR/embebidos-17-2/788d264a0adef514dda11da6d7e1153b7ec77506/practicas/practica1/LuisEGR/img/via_ssh.jpg "LRaspberry Pi SSH")


### 3.- Vía UART - Serial ###

En cuanto a la conexión por UART solo hay que modificar el archivo */dev/config.txt* para habilitar la conexión por UART, haciendo uso de un módulo FT232 conectamos a otra computadora, o a otra raspberry en nuestro caso, y mediante el comando *screen* tenemos acceso a la terminal de nuestra tarjeta.


![RaspberryUART1](https://raw.githubusercontent.com/LuisEGR/embebidos-17-2/master/practicas/practica1/LuisEGR/img/serial1.jpg "UART1")

![RaspberryUART2](https://raw.githubusercontent.com/LuisEGR/embebidos-17-2/master/practicas/practica1/LuisEGR/img/serial2.jpg "UART2")

### Fin ###
![Perro](https://raw.githubusercontent.com/LuisEGR/embebidos-17-2/788d264a0adef514dda11da6d7e1153b7ec77506/practicas/practica1/LuisEGR/img/perro.jpg "#TeamPerro")


## Integrantes ##

* Ávila Flores Felix Alejandro
* González Rodríguez Luis Enrique
* Valdez Sanchez Eduardo Alexeik
* *Héctor Iván Hernández Castelán (oyente)*
* *Lino Cadena Francisco Suriel (oyente)*



## 😁
