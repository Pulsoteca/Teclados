# Corne V4

Fuente original: https://github.com/foostan/crkbd



## Cómo ingresar al Boot Mode

```diff
-- DEBES FLASHEAR EL LADO IZQUIERDO Y DERECHO POR SEPARADO
```

Para actualizar el firmware primero hay que poner el board en boot mode. Para esto hay tres maneras (recomendamos el método 3).


#### Boot Mode Método 1:

1. Desconectar el teclado (Desconectar el USB y TRRS)
2. Mantener Presionado el botón que dice "BOOT" (ver círculo rojo)
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/4770d8b6-e073-4fb3-981b-d05e4b2280d7)

3. Conectar el USB-C mientras el botón de BOOT está presionado.
4. Si todo salió bien, tu computadora debería mostrar el teclado como un dispositivo de almacenamiento.
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/b2284a02-ac47-45ba-89d1-4181e093f672)



#### Boot Mode Método 2:

1. Conectar el teclado con el cable USB-C y desconectar el cable TRRS
2. Mantener Presionado el botón que dice "BOOT" y mientras este está presionado, presionar el botón de RESET (junto al botón de BOOT)
3. Si todo salió bien, tu computadora debería mostrar el teclado como un dispositivo de almacenamiento.

#### Boot Mode Método 3:

1. Desconectar el teclado (Desconectar el USB y TRRS)
2. Mantener Presionado el botón señalado en el círculo rojo (según la parte izquierda o derecha del teclado) y mientras este está presionado, conectar el cable USB-C
   ![image](https://github.com/Pulsoteca/Teclados/assets/167834957/f04cd214-d64f-43ee-a607-fa1673878d9c)

3. Si todo salió bien, tu computadora debería mostrar el teclado como un dispositivo de almacenamiento.


## Como flashear el firmware
```diff
-- DEBES FLASHEAR EL LADO IZQUIERDO Y DERECHO POR SEPARADO
```

El Corne V4 viene con un microcontrolador RP2040 que puede ser flasheado con archivos .u2f

Una vez con el teclado en boot mode, solo debes copiar el archivo .u2f al dispositivo de almacenamiento. De momento hay dos versiones disponibles, una compatible con VIA y otra compatible con VIAL. Si quieres compilar el firmware tu mismo visita el github de foostan para descargar el source code.

* [Firmware para VIA](https://github.com/Pulsoteca/Teclados/blob/main/corne_v4/firmware/crkbd_rev4_standard_via.uf2)
* [Firmware para VIAL](https://github.com/Pulsoteca/Teclados/blob/main/corne_v4/firmware/crkbd_rev4_standard_vial.uf2)

