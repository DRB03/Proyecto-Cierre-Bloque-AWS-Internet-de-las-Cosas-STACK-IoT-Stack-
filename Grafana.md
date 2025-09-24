# Daniel Romero Bravo
## Documentación de  Práctica: Instalación de Grafana en AWS

<img width="512" height="256" alt="image" src="https://github.com/user-attachments/assets/71156c71-eae3-4ce8-94f3-17593c98def1" />

### Instalar Grafana
Se conecta a la instancia EC2 y se instala el software de Grafana utilizando el gestor de paquetes de la distribución Linux (como yum o apt), descargándolo desde los repositorios oficiales de Grafana para garantizar la versión correcta.
<img width="1919" height="933" alt="image" src="https://github.com/user-attachments/assets/a7270f73-66d4-4958-ab5e-d50a9a3c3310" />

### Finalizar Configuración de Grafana y Acceder a la interfaz
Se inicia el servicio de Grafana y se configura para que se ejecute automáticamente al inicio del sistema. Luego, se accede a la interfaz web de Grafana a través del navegador usando la IP pública y el puerto predeterminado (3000) para completar el acceso inicial.
<img width="1916" height="1072" alt="image" src="https://github.com/user-attachments/assets/f8b450af-3098-4141-b05e-e6098c433089" />

### Configurar Data Sources en Grafana
Dentro de la interfaz web de Grafana, se añade y configura una "Fuente de Datos" (Data Source). Esto typically implica conectar Grafana con Prometheus (previamente instalado) especificando la URL donde Prometheus está escuchando, para que Grafana pueda obtener las métricas y crear dashboards.
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/277df093-aac9-49b7-a9a7-49d4dc2708a0" />


