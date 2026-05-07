En este laboratorio se simuló un escenario de ataque SSH en Kali Linux mediante un script creado con nano, el cual generaba intentos de conexión hacia una IP objetivo.

Estos intentos quedaron registrados en un archivo de logs, donde se almacenó toda la actividad resultante de la simulación.

Posteriormente, se realizó un análisis del archivo utilizando cat para visualizar todos los eventos generados. A continuación, se aplicó grep "accepted password" para filtrar posibles autenticaciones exitosas dentro del registro.

El objetivo del ejercicio fue practicar la identificación y análisis de actividad sospechosa en logs, aplicando técnicas básicas de threat hunting en un entorno controlado.
