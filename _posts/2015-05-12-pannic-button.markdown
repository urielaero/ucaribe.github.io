---
title:  "Pannic Button"
subtitle: "kit para monitoreo en casos de alerta"
author: "Pannic button team"
avatar: "img/authors/wferr.png"
image: "img/pannic_button/logo.png"
date:   2015-05-12 12:12:12
---

## Introducción 
Pannic Button es una herramienta de acción-preventiva que ayuda al usuario tener la capacidad de sentirse acompañado todo el tiempo de sus familiares o amigos sin estar en el mismo lugar.

El propósito de la aplicación y wearable es brindar comodidad y seguridad al usuario de poder compartir su ubicación cuando este se sienta amenazado o sienta que está ante un peligro, o inclusive si solo quiere agregar una capa más de seguridad en su travesía a casa, a la escuela o al trabajo.

Pannic Button cuenta con dos partes: un wearable (desarrollado con Adafriut Flora) que el usuario porta y activa una aplicación en Android que envía la ubicación en tiempo real a un servidor web; la segunda parte, la aplicación web, recibe esta ubicación y pinta en un mapa, también en tiempo real, la ubicación del usuario al familia o amigos que este haya seleccionado.

### Tecnología usada
1. Adafruit Flora: usado para el desarrollo del wearable que porta el usuario; este se activará con un movimiento específico hecho por el portador.
2. Android: se desarrolló una aplicación móvil con el propósito de identificar la señal de alerta del portador y envía, cuando se haya invocado dicha alerta, la ubicación actual del usuario.
3. Módulo Bluetooth: incrustado en el Flora y sirve de conexión entre el wearable y el dispositivo Android.


### Modo de uso. 
1. Se instala la aplicación al teléfono con Android.
    <img class="image-center" src="img/pannic_button/p1.png"/>
2. Se coloca la muñequera y se enciende el dispositivo con Flora.
    <img class="image-center" src="img/pannic_button/p2.jpg"/>
3. Se procede a activar el bluetooth del teléfono y la localización GPS.
    <img class="image-center" src="img/pannic_button/p3-1.png"  style="display:inline"/>
    <img class="image-center" src="img/pannic_button/p3-2.png"/ style="display:inline">
4. Se configura el correo que se quiere notificar, a este correo se le enviará un link cuando se active la alerta y podrá ver la localización actual del portador del teléfono.
    <img class="image-center" src="img/pannic_button/p4.png"/>
5. Se activa la conexión del teléfono con el dispositivo Flora.
    <img class="image-center" src="img/pannic_button/p5.png"/>
6. Cuando la conexión se realice, la aplicación android pasa al modo espera.
    <img class="image-center" src="img/pannic_button/p6.png"/>
7. Cuando se realice el movimiento de alerta con el brazo, el teléfono vibra, recibe una notificación, comienza a localizar al teléfono y le envía un correo a la dirección configurada con un enlace para que pueda ver las coordenadas en un mapa interactivo, al hacer click a la notificación se puede desactivar el modo de alerta.
    <img class="image-center" src="img/pannic_button/p7.png"/>
8. El correo configurado recibe el enlace y al presionarlo puede ver lo siguiente.
    <img src="img/pannic_button/p8.png"/ style="width:100%;">



### Movimiento que activa la alerta
<iframe width="560" height="315" src="https://www.youtube.com/embed/yP1y_2RMhtk" frameborder="0" allowfullscreen></iframe>

### Envio del correo con el enlace para comenzar la localización
<iframe width="560" height="315" src="https://www.youtube.com/embed/0C7KsCKBKVA" frameborder="0" allowfullscreen></iframe>

#### Lenguajes de programación usados:
* Elixir: servidor que proporciona un API para almacenar las distintas coordenadas. [Ver repositorio](https://github.com/urielaero/pannic_server)
* Arduino: usado para programar la Flora para detectar el movimiento de alerta. [Ver repositorio](https://github.com/urielaero/pannic_flora)
* Java: usado para el desarrollo de la aplicación móvil. [Ver repositorio](https://github.com/urielaero/android_pannic)
* JavaScript: la interfaz gráfica de la aplicación web se encuentra en esta tecnología. [Ver repositorio](https://github.com/BrandoIsNotASword/panic-button)

#### Equipo:
    Pérez Pacheco Brando 
    Tzel Ciau Antony Uriel 
