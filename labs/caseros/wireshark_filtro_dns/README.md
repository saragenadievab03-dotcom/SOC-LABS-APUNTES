Objetivo

Analizar tráfico de red con Wireshark aplicando filtros DNS para identificar y comparar consultas de dominios legítimos y dominios inexistentes o sospechosos.

Herramientas utilizadas

* Wireshark
* Kali Linux

Procedimiento

Se inició una captura de tráfico en Wireshark y se aplicó el filtro dns para visualizar únicamente paquetes relacionados con el protocolo DNS. Se realizaron consultas a diferentes dominios para generar tráfico de red.

Tráfico generado

* google.com (dominio legítimo con resolución correcta)
* prueba12345.com (dominio inexistente/sospechoso con respuesta NXDOMAIN)

Análisis

Mediante el filtro DNS en Wireshark se aislaron las consultas y respuestas del protocolo, permitiendo observar en tiempo real cómo se resuelven los nombres de dominio y detectar diferencias entre respuestas válidas y no válidas.

Conclusión

El uso de filtros en Wireshark facilita el análisis del tráfico DNS y permite identificar rápidamente resoluciones correctas y dominios inexistentes dentro de la red.
