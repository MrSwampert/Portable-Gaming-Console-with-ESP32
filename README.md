# Portable-Gaming-Console-with-ESP32
Portable Gaming Console with ESP32-WROVER, TFT Display, and MicroSD Storage

Adaptado y diseñado en Altium
# Enlace del repositorio base V1: https://github.com/pebri86/esplay_micro_hardware

# Enlace de la V2: https://www.makerfabs.com/esplay-micro-v2.html

Tengo que hacer una nota de aplicación, en la cual yo busque un repositorio en donde ya haya un proyecto de la consola de juegos basado en el ESP32, que tenga el diagrama de bloques y el título, y los demás archivos. Pero lo importante es tener título, descripción, diagrama de bloques y Power Budget.


# Apuntes:

Escoger uno de los proyectos de consolas de juegos basado en ESP32 (algún repositorio bueno)


Que se puede implementar:

- A ese diagrama de bloques le puedo meter protecciones contra sobrecarga, por ejemplo. 

- Un led que permita saber cuando está cargando y cuando está cargado.

- Si no tiene, se le puede añadir un filtro de condensadores de desacoplo (como está en el diseño del USB Tester) del regulador al MCU.



En la descripción iría lo siguiente (algo así, dependiendo de lo que se le implemente adicional):

"Al diseño original se le realizaron mejoras en cuanto a protección y usabilidad, como la incorporación de un circuito de protección contra sobrecorriente y un sistema de doble LED que informa tanto el estado de carga como el nivel de batería baja. Estas mejoras no solo aumentan la seguridad del dispositivo, sino que también optimizan la experiencia del usuario final."

• El power budget que es?
El power budget es la información del consumo típico de cada componente en V y mA en modo activo.


• El diagrama de bloques que es?

El diagrama de bloques es la información de los componentes y como se comportan en el circuito.

El puerto de micro SD, tiene que ir conectado al RX y TX del MCU

Mirar como es el flujo de conexión de cada periférico que llevará la consola (cruceta, buzzer, micro SD, oled, etc...)

# Componentes:

MCU ESP32 WROVER, Dual core processor with Integrated 4MB Flash + 4MB PSRAM Integrated WIFI and Bluetooth 4 BLE

DISPLAY 2,4" ILI9341 TFT 

CONVERSOR BUTTONS (expanded via PCF8574 I2C GPIO)

PUSH BUTTONS PULSADOR 4 PINES TIPO SMD 6X6X5MM

SWITCH ON/OFF Mini Switch Interruptor Corredera 3 Pines 2 Posiciones 

MICRO SD CONNECTOR slot connected to SDMMC Host in 1 Line Mode for save GPIO pin

DAC (CONVERSOR ANÁLOGO - DIGITAL) CONVERSOR UDA1334A Integrated I2S DAC via UDA1334A

USB TO UART CONTROLLER C FEMALE CH340C

CHARGER MICROCHIP LTC4054 Li-Po charger

LDO REGULATOR LM1117-3.3

I2C PORT EXPANDABLE FUNCTION

3,5mm HEADPHONE JACK

SMALLER SIZE, PCB ONLY 100 x 50 mm

# Enlaces

LDO REGULATOR
https://electronilab.co/tienda/ams1117-3-3-regulador-smd-de-3-3-v-sot-223/

Socket MicroSD: CONECTOR MICRO SD TF PUSH PUSH SMD PCB HOLDER ADAPTADOR
https://ssdielect.com/almacenamiento-de-datos/4367-push-push-sd-card-holder.html

USB C FEMALE: SHOU HAN TYPE-C 16PIN 2MD(073)
https://lcsc.com/product-detail/USB-Connectors_SHOU-HAN-TYPE-C-16PIN-2MD-073_C2765186.html

CIRCUITO DE CARGA (chip de carga): TP4056
https://ssdielect.com/reguladores-de-voltaje-variables/4173-tp4056-chip.html

Batería: Bateria Recargable en Polimero de Litio 3.7V - 1000mA
https://ferretronica.com/products/bateria-recargable-en-polimero-de-litio-3-7v-1000ma

Switch ON/OFF: Mini Switch Interruptor Corredera 3 Pines 2 Posiciones 
https://ferretronica.com/products/mini-switch-interruptor-corredera-3-pines-2-posiciones

Pulsadores (Para la cruceta, botones AB, START y SELECT: x8): PULSADOR 4 PINES TIPO SMD 6X6X5MM
https://ssdielect.com/pulsadores/3285-pulsador-smd-6x6x5mm.html

Amplificador de sonido: Transistor NPN 2N2222
