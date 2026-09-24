# Políticas y Protocolos de Seguridad del Sistema[cite: 2]

## 1. Control de Accesos y Roles (RBAC)[cite: 2]
El sistema aplica un esquema de Control de Acceso Basado en Roles para restringir operaciones sensibles:[cite: 2]
* **Rol Cliente:** Acceso únicamente a lectura de productos y gestión de su propio carrito.[cite: 2]
* **Rol Pasarela de Pagos:** Integración vía tokens cifrados para procesamiento de cobros.[cite: 2]
* **Rol Administrador:** Acceso total a reportes, facturación y modificación de inventario.[cite: 2]

## 2. Encriptación de Datos Sensibles[cite: 2]
* Todas las contraseñas de los usuarios se almacenan encriptadas con el algoritmo **Bcrypt** (factor de costo 10).[cite: 2]
* Todas las transmisiones web se ejecutan obligatoriamente sobre el protocolo **HTTPS (TLS 1.3)**.[cite: 2]

## 3. Autenticación mediante Tokens[cite: 2]
* La API emite firma digital mediante **JWT (JSON Web Tokens)** con tiempo de vida útil de 8 horas.[cite: 2]