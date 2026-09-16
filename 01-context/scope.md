# Servi Te&Pro — Alcance

## Límite del sistema

Servi Te&Pro es una plataforma web orientada a la gestión de solicitudes de asistencia técnica vehicular en el departamento del Huila, Colombia.

Su responsabilidad principal es facilitar el proceso mediante el cual un cliente reporta una avería de su vehículo, proporciona información sobre los síntomas observados, recibe una orientación diagnóstica preliminar y puede ser conectado o asignado a un técnico o profesional que pueda atender la solicitud.

El flujo principal del sistema contempla:

**Cliente → Solicitud → Síntomas → Diagnóstico preliminar → Técnico → Asistencia → Resultado**

El diagnóstico preliminar constituye una orientación basada en las reglas definidas en el sistema y no reemplaza la evaluación técnica realizada directamente por el profesional.

---

## Incluido en el MVP

### Gestión de usuarios

* Registro de usuarios.
* Inicio de sesión.
* Recuperación de contraseña, si se incluye en la implementación inicial.
* Gestión de roles.
* Gestión básica del perfil de usuario.

### Gestión de clientes

* Registro y actualización del perfil del cliente.
* Registro de vehículos.
* Consulta de vehículos registrados.
* Gestión de solicitudes de asistencia.
* Consulta del historial de solicitudes.
* Consulta del estado de las solicitudes.

### Gestión de técnicos

* Registro de técnicos o profesionales.
* Gestión del perfil profesional.
* Registro de especialidades.
* Registro de experiencia profesional.
* Registro de información profesional relevante.
* Configuración de disponibilidad.
* Definición del área de cobertura.

### Gestión de vehículos

* Registro de información básica del vehículo.
* Asociación del vehículo con su propietario.
* Consulta y actualización de la información del vehículo.
* Asociación del vehículo con las solicitudes de asistencia.

### Gestión de solicitudes de asistencia

* Creación de solicitudes por parte del cliente.
* Asociación de la solicitud con un cliente.
* Asociación de la solicitud con un vehículo.
* Registro de la avería reportada.
* Registro de síntomas y características observadas.
* Registro de información adicional proporcionada por el cliente.
* Registro de ubicación de la solicitud cuando sea necesario.
* Adjuntar fotografías como evidencia, si esta funcionalidad se encuentra contemplada en la implementación.
* Consulta y gestión de solicitudes por parte del técnico.
* Asignación o aceptación de una solicitud por parte de un técnico.
* Gestión del estado de la solicitud.
* Registro de la finalización de la asistencia.

### Diagnóstico preliminar

* Análisis de los síntomas registrados por el cliente.
* Aplicación de reglas de diagnóstico previamente definidas.
* Generación de una orientación diagnóstica preliminar.
* Identificación de posibles causas o tipos de avería.
* Identificación de la especialidad técnica que podría ser requerida.
* Presentación del diagnóstico preliminar al técnico como información de apoyo.

El diagnóstico generado por el sistema debe considerarse una orientación inicial. La confirmación de la avería corresponde al técnico durante la atención del vehículo.

### Gestión de la asignación

* Identificación de técnicos que puedan atender una solicitud.
* Consideración de la especialidad requerida.
* Consideración de la disponibilidad del técnico.
* Consideración del área de cobertura.
* Vinculación de la solicitud con el técnico seleccionado o que la acepte.

Los criterios específicos de asignación serán definidos posteriormente como reglas de negocio.

### Gestión de asistencia

* Actualización del estado de la solicitud durante la atención.
* Registro de inicio de la asistencia.
* Registro del resultado de la atención.
* Registro del diagnóstico realizado por el técnico.
* Registro de observaciones técnicas relevantes.
* Consulta del historial de asistencia.

### Administración

* Gestión de usuarios.
* Gestión de técnicos.
* Gestión de especialidades.
* Gestión de solicitudes.
* Gestión de reglas de diagnóstico.
* Gestión de estados y configuraciones básicas.
* Consulta de información necesaria para la administración del sistema.
* Registro de acciones administrativas críticas cuando sea requerido.

### Geolocalización

* Registro de la ubicación asociada a una solicitud de asistencia.
* Registro del área de cobertura del técnico.
* Consideración de la ubicación para la búsqueda o asignación de técnicos.
* Consulta de información geográfica necesaria para el funcionamiento del servicio.

La implementación específica de funcionalidades de geolocalización se definirá durante el diseño de la arquitectura.

---

## Fuera del alcance del MVP

Las siguientes funcionalidades no forman parte del primer MVP de Servi Te&Pro:

* Gestión hotelera.
* Gestión de habitaciones.
* Reservas de alojamiento.
* Gestión de estadías.
* Planificación turística.
* Asistencia turística inteligente.
* Recomendaciones turísticas.
* Guías turísticas.
* Marketplace de repuestos.
* Venta directa de productos físicos.
* Sistema completo de contratación laboral.
* Aplicaciones móviles nativas.
* Expansión fuera del departamento del Huila.
* Soporte multidioma.
* Inteligencia artificial avanzada.
* Diagnóstico automático mediante análisis de imágenes.
* Realidad aumentada.
* Predicción avanzada de demanda.
* Precios dinámicos.
* Integración con compañías de seguros.
* Integración con servicios externos que no sean necesarios para el funcionamiento del MVP.

Estas funcionalidades podrán evaluarse como posibles evoluciones futuras, pero no deben incorporarse al MVP sin una decisión formal de alcance.

---

## Pagos

Los pagos no forman parte del núcleo funcional del MVP.

El sistema podrá quedar preparado para registrar información relacionada con el estado de un pago cuando sea necesario para el flujo de asistencia.

La integración con una pasarela de pagos externa podrá considerarse en una versión futura.

La implementación de pagos deberá tratarse como una funcionalidad independiente y requerirá la definición de sus correspondientes requisitos funcionales, de
