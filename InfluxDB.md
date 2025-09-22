# Daniel Romero Bravo
## Documentación sobre Práctica: Uso actualizado de InfluxDB en Sensores, IoT y Nuevas Tecnologías
<div align="center">
  <img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/c79f3d99-15df-4b2e-93f8-49c8261e7cd8" />
</div>

### Conexión SSH y Preparación del Sistema
Primero me conecté a la instancia EC2 de AWS mediante SSH para tener acceso al servidor donde instalaría InfluxDB. Una vez dentro, actualicé los paquetes del sistema para asegurar que todo esté currente antes de comenzar la instalación.

### Instalación de InfluxDB 2
Procedí a instalar la versión más reciente de InfluxDB 2.0 utilizando el repositorio oficial, descargando e instalando los paquetes necesarios para tener el servidor de base de datos listo en el sistema.
<img width="1249" height="1014" alt="image" src="https://github.com/user-attachments/assets/49481ffc-1fa3-46b7-9fd5-b247c3b8a687" />

### Comprobación de Version
Verifiqué que la instalación se completó correctamente ejecutando el comando de versión, confirmando que tenemos InfluxDB 2.x instalado y disponible para su configuración.
<img width="1247" height="59" alt="image" src="https://github.com/user-attachments/assets/3ba8c36c-9dd4-4397-a4f4-4dfb460679ec" />

### Habilitación y Arranque del servicio
Activé el servicio de InfluxDB para que se inicie automáticamente con el sistema y luego inicié el servicio inmediatamente para poder trabajar con él sin necesidad de reiniciar la instancia.
<img width="1252" height="633" alt="image" src="https://github.com/user-attachments/assets/338ee9e2-67ff-496e-9401-9eaba955a206" />

### Configuración inicial (influx setup)
Ejecuté el comando de configuración inicial que guía through el proceso de setup, donde creé la organización, bucket de datos, usuario administrador y contraseña para el acceso a la instancia de InfluxDB.
<img width="1255" height="405" alt="image" src="https://github.com/user-attachments/assets/fcbf253a-e8e2-42cf-93a2-d053ca9dff74" />

### Ejecución de comandos utiles
Probé comandos esenciales como influx ping para verificar la conectividad con el servidor, y influx bucket list para confirmar la creación correcta del bucket de datos por defecto.
<img width="1252" height="321" alt="image" src="https://github.com/user-attachments/assets/475ad6f0-9645-427c-96b9-cccc77944157" />

### Seguridad: Security Group y UFW
Configuré el Security Group de AWS para permitir el puerto 8086 (puerto default de InfluxDB) y activé UFW (Uncomplicated Firewall) en la instancia para restringir el acceso únicamente a los puertos necesarios, enhancing la seguridad del servidor.
<img width="1247" height="847" alt="image" src="https://github.com/user-attachments/assets/a7ffb0e3-8be6-4d62-93c1-50282faa4018" />

### Creacion de Ejemplo práctico (flujo IoT sencillo)
Desarrollé un script Python simple que simula un dispositivo IoT enviando datos de temperatura y humedad a InfluxDB, demostrando el flujo básico de datos desde un sensor hacia la base de datos temporal.
<img width="1257" height="862" alt="image" src="https://github.com/user-attachments/assets/6029e3d7-5c90-4a22-9aae-0b5f5a6f337c" />

### Ejecución y verificación 
Finalmente, ejecuté el script Python y verifiqué en la interf web de InfluxDB que los datos se estaban almacenando correctamente en el bucket designado, confirmando que todo el flujo IoT funciona adecuadamente.
<img width="1257" height="1014" alt="image" src="https://github.com/user-attachments/assets/1c24aa6e-e655-498e-b5af-794f9ed45b49" />






