# BADGE FIT 10 AÑOS

![](/img/badge.PNG)
![](/img/badge2.jpeg)

Badge FIT 10 años es una tarjeta electrónica diseñada por Ángel Isidro diseñador de dispostivos IoT en el laboratorio de investigación y desarrollo Tesla Lab de Universidad Galileo.

Este dispositivo contiene lo siguiente:
- ESP32
- BME280
- MMA8425QT (Acelerómetro/Giróscopio)
- Matriz Led 8x8
- LiPo Charger

# ¿Cómo funciona?

El Badge funciona por medio de un microcontrolador ESP32 el cual posee conectividad WiFi y BLE, podemos desplegar caracteres por medio de una matriz de Led de 8x8 por medio de conexión SPI, obtiene mediciones de temperatura, humedad y presión atmosférica por medio del sensor BME280, algunas de las aplicaciones puede incluir el uso del Giróscopio.

# ¿Qué podemos hacer?

Enviar datos a un servidor web por medio de WiFi para lo cual necesitaremos conectividad WiFi y crear nuestro servidor Web, publicar datos ambientales en dashboards por medio de MQTT en plataformas como [adafruitIO][adafruit_io].

[adafruit_io]: https://io.adafruit.com
Podemos usar la matriz para desplegar caracteres y mensajes, poseen entradas GPIO para conectar mas dispositivos con el ESP32. 

# Ejemplos con MicroPython 

Para utilizar micropython con nuestro badge visite el siguiente repositorio para mayor información  [FunPython Ecuador][FPE].

[FPE]: https://github.com/FunPythonEC/FIT_Guatemala_2019-SMART_BADGE
