# Nodo Meshtastic ESP32 + LoRa (DX-LR20)

Placa PCB personalizada diseñada específicamente para funcionar como un nodo de la red **Meshtastic**. Combina el microcontrolador **ESP32** con el módulo LoRa **DX-LR20** en un formato ultracompacto, optimizado para uso portátil y alimentación autónoma. 

## ⚡ Especificaciones de Hardware
* **Microcontrolador:** ESP32 (DevKitV1)
* **Radio LoRa:** Módulo DX-LR20
* **Gestión de Energía:**
  * Batería recomendada: Li-Po (ej. 103040 o 656090 a 3.7V)
  * Módulo de carga externo: TP4056
  * Elevador (Boost): MT3608 (a 5V)
  * Regulador Lineal (LDO): AMS1117-3.3V
* **Interfaz de Usuario:**
  * Pulsador (User Button) en el pin `D15` (GPIO15) con Pull-Up por software (preparado para la navegación de la interfaz Meshtastic).
* **PCB:** 2 capas, FR4 TG135, acabado HASL.

## 🔌 Conexiones Principales
* **Alimentación (JST-XH 2.54mm):** Entrada de voltaje desde la batería a través del TP4056.
* **Botón de Usuario:** Conectado en configuración *Active Low* entre `GND` y `GPIO15`.

## 📂 Estructura del Repositorio
* `/Hardware`: Archivos Gerber listos para enviar a fábrica, esquemas en PDF y lista de materiales (BOM).
* `/Software`: Archivos de configuración o notas sobre la versión del firmware de Meshtastic utilizada.
* `/3D_Model`: Archivos STL/STEP de la carcasa de bolsillo (incluyendo espacio para la batería y antena).

## 🚀 Estado del Proyecto
- [x] Diseño del esquemático eléctrico.
- [x] Enrutado de la PCB y optimización de planos de masa.
- [x] Fabricación de la PCB.
- [x] Flasheo y configuración del firmware Meshtastic.
- [ ] Diseño e impresión 3D de la carcasa.