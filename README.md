# Modulo-Uplynx-de-M2COMM #
Proyecto para aprender a utilizar el modulo Uplynx RCZ2 de M2COMM por medio de comandos AT a través de una terminal. Una vez familiarizado con las instrucciones propias del módulo, se utilizará el programa M2C_Uplynx para crear pequeños programas para posteriormente guardarlo en el MCU del módulo M2COMM. 

## Equipo y software necesario ##
<br />
-Módulo Uplynx RCZ2 de M2COMM.
<br />
![modulo_m2comm](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/modulo_m2comm.png?raw=true)
<br />
-Software para emular una Terminal en Windows (Tera Term, PuTTy, KiTTy, etc).
<br />
-Una cuenta en Sigfox. Para México puedes obtener una cuenta escribiendo al correo contacto@iotnet.mx

## Primeros pasos ## 
Antes que nada, debemos conocer los comandos AT del módulo M2COMM. A continuación se presentan algunos de ellos:

![modulo_m2comm](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/comandos1.png?raw=true)

Cabe destacar algunos comandos importantes como:
<br />
-AT$ID?: regresa el ID del dispositivo.
<br />
-AT$PAC?: regresa el PAC.

(Leer la hoja de datos del módulo para conocer más sobre las especificaciones técnicas y la lista completa de comandos AT.)


Una vez que se conocen los comandos AT que nos permitirán comunicarnos con la tarjeta, se procede a la configuración de la misma.

Conectar la tarjeta a un puerto USB de manera que los jumpers estén conectados en “POWER_EN Enable(Pc)” y “5VUSB”:

![m2comm_5](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_5.jpg?raw=true)

Una vez que Windows termine de instalar los drivers, ir al administrador de dispositivos para saber en que puerto COM está conectada la tarjeta:

![m2comm_2](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_2.png?raw=true)

Cerramos el administrador de dispositivos y ejecutamos Tera Term. Al abrirlo nos mostrará una ventana donde tenemos que configurar el puerto por el que deseamos hacer la conexión. Seleccionamos la opción serial y el puerto y damos click en OK

![m2comm_3](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_3.png?raw=true)

Si todo está correctamente configurado, nos aparecerá el siguiente mensaje en la terminal:

![m2comm_4](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_4.png?raw=true)

Dependiendo del programa utilizado, habrá que configurar el puerto antes de realizar la conexión (Baud rate, data, parity, bit stop), en este caso Tera Term ya lo hace por defecto:

![m2comm_6](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_6.png?raw=true)



