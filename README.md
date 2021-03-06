# BADGE FIT 10 AÑOS

![](/img/badge.PNG)
![](/img/badge2.jpeg)
![](/img/GT000001.svg)

Badge FIT 10 años es una tarjeta electrónica diseñada por Ángel Isidro diseñador de dispostivos IoT en el laboratorio de investigación y desarrollo Tesla Lab de Universidad Galileo.

Este dispositivo contiene lo siguiente:
- ESP32
- BME280
- MMA8425QT (Acelerómetro/Giróscopio)
- Matriz Led 8x8
- LiPo Charger

# ¿Quién obtuvo un BADGE?

Los primeros 100 participantes inscritos en el FIT obtuvieron su BADGE conmemorativo a los 10 años del evento.

# ¿Cómo funciona?

El Badge funciona por medio de un microcontrolador ESP32 el cual posee conectividad WiFi y BLE, podemos desplegar caracteres por medio de una matriz de Led de 8x8 por medio de conexión SPI, obtiene mediciones de temperatura, humedad y presión atmosférica por medio del sensor BME280, algunas de las aplicaciones puede incluir el uso del Giróscopio.

# ¿Qué podemos hacer?

Enviar datos a un servidor web por medio de WiFi para lo cual necesitaremos conectividad WiFi y crear nuestro servidor Web, publicar datos ambientales en dashboards por medio de MQTT en plataformas como [adafruitIO][adafruit_io].

[adafruit_io]: https://io.adafruit.com
Podemos usar la matriz para desplegar caracteres y mensajes, poseen entradas GPIO para conectar mas dispositivos con el ESP32. 

# Ejemplos con MicroPython 

Para utilizar micropython con nuestro badge visite el siguiente repositorio para mayor información  [FunPython Ecuador][FPE].

[FPE]: https://github.com/FunPythonEC/FIT_Guatemala_2019-SMART_BADGE

# Descripción de pines 

### Temperatura, humedad y presión atmosférica - Comunicación I2C
ESP32 | BME280
--- | ---
SCL 22 | SCK 4
SDA 23 | SDI 3

### Acelerómetro/Giróscopio - Comunicación I2C
ESP32 | MMA8425QT
--- | ---
SCL 22 | SCL 4
SDA 23 | SDA 6

### Matriz led 8x8 - Comunicación SPI
ESP32 | MAX7219CWG
--- | ---
5V | VCC 
GND | GND
MOSI 16 | DIN 1
CS 17 | CS 12
SCK 21 | CLK 13

# Licencia

Hardware License: CERN OHL v1.0 para más información visitar el siguiente [Link][CERN_v1].

[CERN_v1]: https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-1.2

Software License: GPL v3

Documentation License: CC BY 4.0 International
