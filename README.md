# Biomedical Signal Sensors (Wi-Fi streaming + Python analysis)

Proyecto para **adquirir y analizar señales biomédicas** enviadas por un microcontrolador vía Wi-Fi hacia una PC en la misma red.  
La señal se transmitió en tiempo real, se guardó en Excel/CSV y luego se analizó en Python.

## 🧩 Arquitectura (pipeline)
1) **Sensor**: pulso (y/o flex) → entrada analógica del microcontrolador  
2) **Microcontrolador con Wi-Fi**: ESP32/ESP8266 (o similar)  
3) **Transmisión**: envío por UDP/TCP a la **IP de la PC** en la red local  
4) **PC (servidor/receptor)**: captura y guarda datos en **CSV/Excel**  
5) **Python**: lectura del CSV → filtrado → métricas → gráficos

