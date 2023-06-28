# Ficheros3D_STEP_EN_ATLAS Y mejoras en el diseño actual de "LA ROJA"
Compartir ficheros STEP en tres dimensiones, para montajes de diseños ATLAS.

El objetivo de ATLAS siempre ha sido poscionarse como una opción openhardware de aprendizaje tanto de microntroladores, SBCs, CPLDs, y FPGAS, en un rango de precios inferior a los 50€

Otro de los objetivos de esta entrada es disponer de modelos tridimensionales para el ensamblaje de la placa I/O Board ATLAS Mini, así como mostrar la nueva míni.

Se muestra un diseño mejorado de la ROJA, en el pantallazo de Kicad, en la que se ve que hay soporte SIO en el bus SBC, el uso de dos mosfet BSS138 para tener una señal I2C en el bus de video digital, y no dañar placas con tensiones de referencia de +3V3, dado que el bus digital usa una tensión de +5V.

A.- Estoy ajustando los pares diferenciales para que sea iguales desde cada par dado que muchos de ellos estan alejados y no estan posicionados correctamente en la CYC1000, supongo que los diseñadores de nunca pensaron en que una placa CYCLONE 10 LP enfocada al usuario de arduino, se usaría para crear pares diferenciales compatibles con DVI a +3V3 porque la dispoción totalmente desordenada de los pines te hace pensar esto mismo.

B.- El video dital DVI posée una traducción de niveles de tensión de +3V3 <---> +5V en su bus I2C, mediante la configuración de un mosfet BSS138.

C.- El bus SIO esta presente en el bus SBC de 2x20 pines.


