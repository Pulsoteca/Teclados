# Corne V4

El contenido mostrado está basado en la fuente original: https://github.com/foostan/crkbd



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



## Como configurar el teclado con VIA

Si flasheaste el firmware con VIA, puedes configurarlo en [VIA App](https://usevia.app)

1. Ingresa a la pagina [VIA App](https://usevia.app)
2. Ve a la pestaña de design y da click en Load
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/0dc1b311-1bed-4767-b781-f33c2310b2e4)
3. Carga el archivo .json con el layout: [Link al archivo .json](https://github.com/Pulsoteca/Teclados/blob/main/corne_v4/layouts/crkbd_rev4.json)
4. Si todo salió bien, deberías de ver el layout cargado:
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/a3ca63cd-d5d8-4ece-9ef6-2bf54fed3584)
5. Vuelve a la pestaña de configure, click en Authorize Device, selecciona tu teclado y click en Connect
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/be7470d5-550c-47de-acf4-80d3a2204134)
6. Si tu teclado está configurado con encoders, deberás especificarlo en el menu de layout, en el ejemplo de bajo se muestra un encoder del lado derecho superior
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/37476b3d-9635-4a53-b1a1-a3cc4c2fee6d)
7. Estás listo para configurarlo
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/f311eb30-5525-4977-93d5-67f858407e00)



 
