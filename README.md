# Proyecto: Notificaciones Diarias del Clima con Twilio y AWS 📡

Este proyecto automatiza el envío diario del pronóstico del clima a través de mensajes SMS usando **Twilio**, datos de **WeatherAPI**, y un script de **Python** ejecutado diariamente con **cron** en una instancia EC2 de **AWS**.
## Tecnología usada en este proyecto: 
_Python 3.12, Twilio API, WeatherAPI, Requests, Pandas, tqdm , cron, Instancia EC2 de AWS (Ubuntu 22.04)_

Cada día, el script obtiene el pronóstico del clima de una ciudad específica y lo envía como mensaje SMS a un número telefónico verificado. El objetivo de este proyecto es integrar automatización, consumo de APIs externas, y servicios de mensajería.

## Estructura del Proyecto 🧩
proyecto_clima/

│

**├── twilio_script.py --------# Script principal**

**├── twilio_config.py -------# Variables sensibles (cargadas desde .env)**

**├── utils.py ----------------# Funciones auxiliares**

**├── .env --------------------# Variables de entorno (no versionar)**

**├── requirements.txt ------# Dependencias**

## ¿Qué hace el script? 🧪

- Consulta el pronóstico del día desde WeatherAPI.
- Formatea la información para lectura humana.
- Envía un SMS con el pronóstico al teléfono configurado.
- Se ejecuta automáticamente todos los días.

## Mensaje recibido mediante SMS:

![WhatsApp Image 2025-06-16 at 21 28 29](https://github.com/user-attachments/assets/0c69a8f3-9675-4ad0-9406-5bf4bee60175)
