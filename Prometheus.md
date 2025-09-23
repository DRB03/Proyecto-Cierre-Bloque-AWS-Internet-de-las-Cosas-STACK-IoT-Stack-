# Daniel Romero Bravo
## Documentación sobre Práctica: Instalación de Prometheus en AWS
<img width="830" height="370" alt="image" src="https://github.com/user-attachments/assets/1969195f-a6fc-487a-959e-9e716bdf05c7" />

### Descargar e Instalar Prometheus
Se conecta a la instancia EC2, descarga los binarios de Prometheus desde su sitio oficial, los descomprime y los coloca en un directorio del sistema (/usr/local/bin/). 

<img width="1919" height="928" alt="image" src="https://github.com/user-attachments/assets/19286a9a-d143-4c2f-9321-e1ada67f6d4f" />
<img width="1919" height="927" alt="image" src="https://github.com/user-attachments/assets/fda53c28-464c-477c-b0c7-f326b75ad5cd" />


### Configurar Prometheus
Se crea un archivo de configuración YAML (prometheus.yml) donde se definen parámetros como la frecuencia de recolección de métricas y los objetivos a monitorear (en este caso, la propia instancia EC2).

<img width="1919" height="927" alt="image" src="https://github.com/user-attachments/assets/e918b3d3-340c-4b96-a8d5-c1d9a0f6225e" />


### Crear Servicio Systemd
Se crea un archivo de servicio (prometheus.service) para que systemd (el administrador de servicios de Linux) pueda iniciar, detener y reiniciar Prometheus automáticamente, asegurando que se ejecute tras un reinicio del sistema.

<img width="1919" height="921" alt="image" src="https://github.com/user-attachments/assets/2e26b1e6-b445-4571-b6f2-a50a8f975fe6" />


### Instalar Node Exporter
Se instala el "Node Exporter", un complemento de Prometheus que se encarga de recolectar métricas del sistema operativo y del hardware de la instancia (como uso de CPU, memoria, disco, etc.).

<img width="1919" height="920" alt="image" src="https://github.com/user-attachments/assets/cff60e66-6435-4cae-ba60-7cd707c54a10" />
<img width="1919" height="929" alt="image" src="https://github.com/user-attachments/assets/810351e5-09fc-4a3d-adb7-0fff59e337e1" />


### Comprobación de Prometheus y Node Exporter
Se verifica que ambos servicios (Prometheus y Node Exporter) estén ejecutándose correctamente. La comprobación final se hace accediendo a la interfaz web de Prometheus desde un navegador usando la IP pública de la instancia para confirmar que esté recolectando métricas.
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/19de7939-3bbe-4f69-aa79-853f8741e84c" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/feb15029-e818-484d-8389-d9164dfa12a0" />












