# Ficheros3D_STEP_EN_ATLAS Y mejoras en el diseño actual de "LA ROJA"
Compartir ficheros STEP en tres dimensiones, para montajes de diseños ATLAS.

El objetivo de ATLAS siempre ha sido poscionarse como una opción openhardware de aprendizaje tanto de microntroladores, SBCs, CPLDs, y FPGAS, en un rango de precios inferior a los 50€

Otro de los objetivos de esta entrada es disponer de modelos tridimensionales para el ensamblaje de la placa I/O Board ATLAS Mini, así como mostrar la nueva míni.

Se muestra un diseño mejorado de la ROJA, en el pantallazo de Kicad, en la que se ve que hay soporte SIO en el bus SBC, el uso de dos mosfet BSS138 para tener una señal I2C en el bus de video digital, y no dañar placas con tensiones de referencia de +3V3, dado que el bus digital usa una tensión de +5V.

---

Imagen tridimensional en Freecad para posibles ensamblados futuros de carcasas.
![ATLAS MINI MEJORADA](https://github.com/AtlasFPGA/Ficheros3D_STEP_EN_ATLAS/blob/main/FOTOS/Captura%20de%20pantalla%20ATLAS%20MINI%20de%202023-06-28%2012-37-38.png)

---

A.- Estoy ajustando los pares diferenciales para que sea iguales desde cada par dado que muchos de ellos estan alejados y no estan posicionados correctamente en la CYC1000, supongo que los diseñadores de nunca pensaron en que una placa CYCLONE 10 LP enfocada al usuario de arduino, se usaría para crear pares diferenciales compatibles con DVI a +3V3 porque la dispoción totalmente desordenada de los pines te hace pensar esto mismo.

B.- El video dital DVI posée una traducción de niveles de tensión de +3V3 <---> +5V en su bus I2C, mediante la configuración de un mosfet BSS138.

C.- El bus SIO esta presente en el bus SBC de 2x20 pines.

---

Visualización modelo Raspberry PI Zero II:
![Frecad Raspberry PI Zero II](https://github.com/AtlasFPGA/Ficheros3D_STEP_EN_ATLAS/blob/main/FOTOS/Captura%20de%20pantalla%20Frecad%20rp%20zw2%20de%202023-06-28%2012-18-27.png)

---

Visualización modelo CYC1000 con PMOD cambiado a PINHEARER 2x8:
![CYC1000 con PMOD cambiado a PINHEARER 2x8](https://github.com/AtlasFPGA/Ficheros3D_STEP_EN_ATLAS/blob/main/FOTOS/Captura%20de%20pantalla%20FreeCAD%20%20de%20la%20placa%20CYC1000%20PARA%20USO%20DE%20LA%20ATLAS%20MINI%20para%20montaje%20carcasa%20%202023-06-28%2012-09-28.png)

---

Añadidos los mosfet BSS138 para realizar una traducción de nivel de las señales I2C
![Añadidos los mosfet BSS138](https://github.com/AtlasFPGA/Ficheros3D_STEP_EN_ATLAS/blob/main/FOTOS/Detalle%20de%20la%20Captura%20de%20pantalla%20donde%20se%20ven%20los%20diodos%20mosfet%20para%20adaptar%20los%20niveles%20de%20tensi%C3%B3n%20del%20bus%20i2c%20de%202023-06-28%2013-06-30.png)

---

Nuevo diseño de ATLAS MINI sin cambiar el formato y con diversas mejoras:

![Nuevo diseño de ATLAS MINI](https://github.com/AtlasFPGA/Ficheros3D_STEP_EN_ATLAS/blob/main/FOTOS/Captura%20de%20pantalla%20de%20la%20ATLAS%20MINI%20MEJORADA%20I2C%20y%20SDIO%202023-06-28%2012-24-34.png)

---
