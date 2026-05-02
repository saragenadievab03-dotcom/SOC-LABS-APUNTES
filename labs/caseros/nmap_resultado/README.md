# Port Scanning Lab 
 
# Objetivo
Identificar puertos abiertos en el sistema y analizar los servicios asociados.

# Herramienta
- Nmap

# Procedimiento
Se realizó un escaneo de puertos sobre localhost utilizando Nmap.

# Resultados
Se detectaron los siguientes puertos abiertos:

- 22/tcp → SSH (OpenSSH)
- 80/tcp → HTTP (Apache)
- 631/tcp → IPP (CUPS)

# Análisis
Los puertos abiertos indican servicios activos en el sistema:

- El puerto 22 permite conexiones remotas (SSH)
- El puerto 80 indica un servidor web activo
- El puerto 631 está relacionado con servicios de impresión

# Conclusión
El escaneo de puertos permite identificar servicios activos y posibles puntos de entrada en un sistema.
