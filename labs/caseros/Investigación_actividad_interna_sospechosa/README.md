 # Suspicious Internal Activity Investigation

# Objetivo
Simular e investigar actividad sospechosa en un sistema Linux desde una perspectiva Blue Team.



# Escenario

Durante una revisión del sistema se detectaron:
- scripts sospechosos
- conexiones externas
- archivos sensibles
- comandos de enumeración



# Actividades detectadas

# Script sospechoso

Se identificó un script llamado:

updater.sh

El script intentaba realizar conexiones HTTP externas mediante curl.



# Archivo sensible

Se detectó un archivo potencialmente sensible:

credentials_dump.txt

El archivo contenía credenciales simuladas.



# Comandos observados

Se identificaron comandos relacionados con enumeración del sistema:
- whoami
- uname
- history



# Investigación realizada

Se analizaron:
- procesos activos
- conexiones de red
- historial bash
- hashes SHA256
- tipos de archivo



# Herramientas utilizadas

- Linux
- curl
- ps
- ss
- sha256sum
- file



# IOC identificados

- malicious-update.com
- updater.sh
- credentials_dump.txt



# Conclusión

El laboratorio permitió practicar investigación básica de actividad sospechosa en Linux desde una perspectiva SOC y Blue Team.
