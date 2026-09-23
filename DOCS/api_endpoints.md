# Especificacion de Endpoints de la API

Esta seccion documenta los servicios web (Web API) disponibles para la integracion con otros sistemas.

## 1. Listado de Servicios Web

| Método HTTP | Ruta / Endpoint | Descripción | Parámetros Exigidos |
| :-: | :--- | :--- | :--- |
|** GET ** | `/api/v1/usuarios` | Obtiene el listado completo de usuarios registrados. | Ninguno |
|** POST ** | `/api/v1/usuarios` | Registra un nuevo usuario en la base de datos. | `nombre`, `correo`,|`rol` |
| ** GET ** | `/api/v1/reportes` | Genera y descarga el reporte mensual en PDF. | `mes` (numerico) |

## 2. Códigos de Respuesta HTTP

> ** Estandar de Errores :** Todos los servicios responden utilizando codigos de estado HTTP estándar.

* ** 200 OK :** La solicitud fue procesada exitosamente.
* ** 400 Bad Request :** Datos de entrada inválidos o faltantes.
* ** 404 Not Found :** El recurso solicitado no existe en el servidor.
* ** 500 Internal Server Error :** Error interno en la lógica de Python o en la base de datos MySQL.

## 3. Ejemplo de Respuesta JSON
```json
{
 "status": 200,
 "message": "Usuario registrado exitosamente",
 "data": {
   "id": 105,
   "nombre": "Carlos López",
   "rol": "Desarrollador"
 }
}
```

## 4. Navegación
- [Ver Manual de Usuario](manual_usuario.md)
- [Ver Arquitectura del Sistema](arquitectura.md)
- [Volver al README Principal](../README.md)