# Documentación de Arquitectura: Casos de Uso

## 1. Descripción del Módulo
El presente documento define los requisitos funcionales del sistema. Se detalla la interacción entre los actores y las funcionalidades del sistema.

## 2. Diagrama UML de Casos de Uso
![Diagrama de Casos de Uso](../assets/casos_de_uso.png)

## 3. Especificación de Relaciones
- **Relaciones <<include>>:** Reservar Cita y Generar Factura requieren obligatoriamente la autenticación previa del usuario en el sistema.
- **Relaciones <<extend>>:** Aplicar Descuento de Seguro se ejecuta únicamente si la factura generada cuenta con cobertura médica.