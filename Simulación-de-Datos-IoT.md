# Daniel Romero Bravo
## Simulación de Datos IoT usando Entorno Virtual Python

### Instalar Python, Crear y Activar Entorno Virtual
Se instala Python y las herramientas necesarias en la instancia EC2. Luego se crea un entorno virtual aislado usando venv (o virtualenv) para gestionar las dependencias del proyecto de forma separada del sistema operativo, y se activa dicho entorno.

<img width="1919" height="924" alt="image" src="https://github.com/user-attachments/assets/6935e35a-c91d-4c08-a6cb-fb75a11c2fa6" />

### Instalar Cliente InfluxDB en el Entorno Virtual
Dentro del entorno virtual activado, se instala la biblioteca cliente de InfluxDB para Python usando pip. Esto permite que los scripts Python puedan comunicarse y enviar datos a una base de datos InfluxDB.

<img width="1919" height="935" alt="image" src="https://github.com/user-attachments/assets/ff643a09-7b87-4efa-95bf-b898bb91e56c" />

### Creación del Dashboard en Grafana
Se accede a la interfaz web de Grafana y se crea un nuevo dashboard personalizado. Aquí se configuran paneles de visualización (gráficos, medidores, etc.) que se conectarán a una fuente de datos (como InfluxDB) para mostrar las métricas en tiempo real de manera visual.

<img width="1919" height="927" alt="image" src="https://github.com/user-attachments/assets/bb2804b7-43b8-4658-99ce-cd259ece7d85" />
<img width="1919" height="927" alt="image" src="https://github.com/user-attachments/assets/9c9f0d2e-3f3d-43c7-b965-a4b3a0d08a32" />

### Ejecucion del Simulador y Prueba de actualizacion por medio de Dashboard 
Se ejecuta un script Python (simulador) que genera datos de prueba y los envía a la base de datos InfluxDB. Simultáneamente, se verifica en el dashboard de Grafana que los paneles se actualicen automáticamente, confirmando que el flujo completo (simulador → InfluxDB → Grafana) funciona correctamente, tambien Adjunto video de evidencia en Loop:

https://www.loom.com/share/9493e3389cbf446696893e9dc7d8c4d0?sid=cb32ec59-ee1e-4cb1-9abd-c8cd8dd2609b
