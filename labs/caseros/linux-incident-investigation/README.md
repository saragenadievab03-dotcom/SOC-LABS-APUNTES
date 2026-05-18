# Linux Incident Investigation 

# Objetivo
Investigar actividad sospechosa en un sistema Linux desde una perspectiva Blue Team.


# Escenario
Durante una revisión del sistema se detectó un script llamado:

updater.sh

El script intentaba realizar conexiones externas utilizando curl.


# Actividades realizadas

# Enumeración de procesos
Se analizaron procesos activos mediante:

bash
ps aux


# Revisión de conexiones
Se investigaron conexiones del sistema utilizando:

bash
ss -tunap


# Identificación del archivo
Se verificó el tipo de archivo con:

bash
file updater.sh

  
# Generación de hash SHA256
Se calculó el hash del archivo:

bash
sha256sum updater.sh


# Análisis

El script realizaba un intento de conexión HTTP hacia un dominio externo utilizando curl.

Este tipo de comportamiento puede observarse en:
- scripts maliciosos
- malware
- herramientas automatizadas

Aunque la conexión no se completó correctamente, el comportamiento fue investigado como actividad potencialmente sospechosa.


# Herramientas utilizadas
- Linux
- curl
- ps
- ss
- file
- sha256sum


# Conclusión
Este laboratorio permitió practicar técnicas básicas de investigación y análisis de actividad sospechosa en Linux desde una perspectiva SOC y Blue Team.
