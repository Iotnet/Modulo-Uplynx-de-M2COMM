# Modulo-Uplynx-de-M2COMM #
Proyecto para aprender a utilizar el modulo Uplynx RCZ2 de M2COMM por medio de comandos AT a través de una terminal. Una vez familiarizado con las instrucciones propias del módulo, se utilizará el programa M2C_Uplynx para crear pequeños programas para posteriormente guardarlo en el MCU del módulo M2COMM.

## Equipo y software necesario ##
<br />
-Módulo Uplynx RCZ2 de M2COMM.
<br />
![modulo_m2comm](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/modulo_m2comm.png?raw=true)
<br />
-Software para emular una Terminal (Tera Term, PuTTy, KiTTy, etc).
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

![m2comm_5](https://github.com/Iotnet/Modulo-Uplynx-de-M2COMM/blob/master/images/m2comm_5.png?raw=true)
 