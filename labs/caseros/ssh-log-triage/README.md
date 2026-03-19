# Lab Casero: Monitoreo de Logs SSH

# Objetivo
El objetivo de este lab es practicar la conexión SSH a un servidor Ubuntu y analizar los logs de autenticación ('auth.log').  
Quiero aprender a identificar accesos correctos y fallidos, entender cómo se registran los eventos en los logs y familiarizarme con tareas básicas de monitoreo que realiza un analista SOC.

# Pasos realizados

# 1. Conexión SSH al servidor
Me conecté desde mi máquina Linux al servidor Ubuntu usando SSH.  
Al ingresar la contraseña correcta, pude acceder y empezar a explorar el entorno.

*Aprendizaje: entendí cómo establecer una conexión segura y qué información se genera al iniciar sesión correctamente.

---

# 2. Visualizar los últimos eventos del log
Dentro del servidor, revisé los últimos eventos de autenticación con 'tail'.  
Esto me permitió ver los accesos recientes y cierres de sesión.

*Aprendizaje: comprendí la estructura de 'auth.log' y la importancia de revisar logs recientes para detectar actividad relevante.

---

# 3. Filtrar solo intentos fallidos
Para enfocarme en accesos incorrectos, utilicé 'grep' para buscar solo los intentos fallidos de login.  
Esto me ayudó a identificar rápidamente si había actividad sospechosa o fallos de autenticación.

* Aprendizaje: aprendí a aislar la información relevante y cómo detectar intentos fallidos de manera eficiente, como lo haría un analista SOC.
  
---

# 4. Monitoreo en tiempo real
Finalmente, monitoricé los eventos de autenticación en tiempo real usando 'tail -f' combinado con filtrado de fallos.  
Mientras tanto, generé un intento fallido desde otra terminal para observar cómo se registraba instantáneamente.

*Aprendizaje: entendí cómo los eventos se registran al instante y cómo un analista SOC puede reaccionar a incidentes en tiempo real. Esto me dio una visión más práctica de la detección de alertas.

---

# Conclusiones y aprendizajes
- Diferenciar entre accesos correctos y fallidos y cómo se reflejan en los logs.  
- Uso de 'tail' y 'grep' para analizar eventos relevantes de manera rápida y efectiva.  
- La importancia de monitorear logs en tiempo real para detectar actividad sospechosa.  
- Este lab me permitió aplicar conceptos básicos de triage de alertas y mejorar mi mentalidad de analista SOC.
