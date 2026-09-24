# Guía de Despliegue e Instalación del Sistema

## 1. Requisitos Previos del Servidor

Para poner en marcha la aplicación e-commerce, se requiere disponer del siguiente entorno:

- **Servidor Web:** Node.js v18.x o superior.
- **Base de Datos:** PostgreSQL v15.0.
- **Memoria RAM Mínima:** 2 GB RAM / 2 Cores CPU.
- **Sistema Operativo:** Ubuntu Server 22.04 LTS (Recomendado).

## 2. Procedimiento de Instalación Técnicamente Despachado

### Paso 2.1: Obtención del Código Fuente

El administrador del sistema debe clonar el repositorio remoto oficial desde la plataforma GitHub hacia el servidor de destino y navegar a la carpeta raíz del proyecto.

### Paso 2.2: Instalación de Dependencias del Proyecto

Se deben instalar los paquetes y dependencias requeridas mediante el gestor de paquetes del entorno Node.js, ejecutando la descarga automática descrita en el archivo de configuración.

### Paso 2.3: Configuración de Variables de Entorno

Crea un archivo llamado `.env` en la raíz del proyecto tomando como base el archivo `.env.example`, definiendo los parámetros de conexión:

- Puerto de red del servicio (`PORT`)
- Dirección de host de la base de datos (`DB_HOST`)
- Puerto de base de datos (`DB_PORT`)
- Usuario y clave de acceso a la base de datos (`DB_USER`, `DB_PASS`)

### Paso 2.4: Puesta en Marcha del Servicio

Iniciar el servicio web en modo de desarrollo o producción verificando en la consola que los puertos de enlace estén abiertos y escuchando peticiones.