# Reviung 53

El contenido mostrado está basado en la fuente original: https://github.com/gtips/reviung

## Cómo ingresar al Boot Mode


Para actualizar el firmware primero hay que poner el board en boot mode. Para esto hay dos maneras.

#### Boot Mode Método 1:

1. Desconectar el cable USB-C del teclado (dejar conectado a la computadora)
2. Mantener Presionada la tecla 'Q'
3. Conectar el teclado con el cable USB-C mientras la tecla 'Q' está presionada.
4. Si todo salió bien, tu computadora debería mostrar el teclado como un dispositivo de almacenamiento.

![image](https://github.com/Pulsoteca/Teclados/assets/167834957/3970444e-3531-4c8c-997d-4b16f1d62e61)


#### Boot Mode Método 2:

1. El teclado debe estar conectado a la computadora con el cable USB-C
2. Mantener Presionada la tecla 'Q'
3. Presionar el botón de reset por la parte trasera
4. Si todo salió bien, tu computadora debería mostrar el teclado como un dispositivo de almacenamiento.

![image](https://github.com/Pulsoteca/Teclados/assets/167834957/4b76ab66-4c19-41c6-9c09-2c898b44182d)


## Como flashear el firmware

El teclado está integrado con un microcontrolador RP2040 que puede ser flasheado con archivos .u2f

Una vez con el teclado en boot mode, solo debes copiar el archivo .u2f al dispositivo de almacenamiento. 

* [Firmware para VIA](https://github.com/Pulsoteca/Teclados/blob/main/reviung53/firmware/reviung_reviung53_via.uf2)

Si quieres compilar el firmware por ti mismo, el source code lo encuentras aquí:

* [Source code](https://github.com/Pulsoteca/Teclados/tree/main/reviung53/firmware/source)



## Como configurar el teclado con VIA

Si flasheaste el firmware con VIA, puedes configurarlo en [VIA App](https://usevia.app)

1. Ingresa a la pagina [VIA App](https://usevia.app)
2. Ve a la pestaña de design y da click en Load
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/0dc1b311-1bed-4767-b781-f33c2310b2e4)
3. Carga el archivo .json con el layout: [Link al archivo .json](https://github.com/Pulsoteca/Teclados/blob/main/reviung53/layouts/reviung53_via.json)
4. Si todo salió bien, deberías de ver el layout cargado:
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/97f11ea6-186a-43a5-8e5f-9f24d737e12d)

5. Vuelve a la pestaña de configure, click en Authorize Device, selecciona tu teclado y click en Connect
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/be7470d5-550c-47de-acf4-80d3a2204134)
6. Si tu teclado está configurado con encoders, deberás especificarlo en el menu de layout, en el ejemplo de bajo se muestra un encoder del lado derecho superior
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/37476b3d-9635-4a53-b1a1-a3cc4c2fee6d)
7. Estás listo para configurarlo
![image](https://github.com/Pulsoteca/Teclados/assets/167834957/f311eb30-5525-4977-93d5-67f858407e00)



 
