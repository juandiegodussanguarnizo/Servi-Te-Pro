# Servi Te&Pro — Descripción General

## ¿Qué es Servi Te&Pro?

Servi Te&Pro es una plataforma web orientada a la solicitud y gestión de servicios de asistencia técnica vehicular en el departamento del Huila, Colombia.

El sistema permite que un cliente registre su vehículo, reporte una avería y describa los síntomas o situación presentada. A partir de esta información, la plataforma puede generar una orientación diagnóstica preliminar basada en reglas y facilitar la identificación o asignación de un técnico o profesional que pueda atender la necesidad reportada.

El proyecto busca mejorar la comunicación entre el cliente y el técnico, proporcionando información relevante antes de realizar la asistencia y facilitando una atención más organizada.

## Problema que resuelve

Cuando un vehículo presenta una avería, el cliente puede no conocer la naturaleza técnica del problema ni saber qué tipo de profesional debe contactar. Además, la información proporcionada al técnico puede ser insuficiente para determinar previamente qué herramientas, conocimientos o recursos podrían ser necesarios para atender la situación.

Esta situación puede generar demoras, asignaciones inadecuadas y desplazamientos innecesarios.

Servi Te&Pro busca centralizar el proceso de solicitud de asistencia, recopilación de síntomas, orientación diagnóstica preliminar y conexión con el técnico correspondiente, con el propósito de facilitar una atención técnica más organizada y pertinente.

## Usuarios principales

* **Cliente:** registra y gestiona sus vehículos, solicita asistencia técnica, proporciona información sobre la avería y sus síntomas, consulta el estado de la solicitud y recibe información relacionada con la atención.

* **Técnico:** gestiona su perfil profesional, registra sus especialidades y disponibilidad, recibe solicitudes de asistencia con la información proporcionada por el cliente y el diagnóstico preliminar generado por el sistema, atiende la solicitud y registra el resultado de la asistencia.

* **Administrador:** gestiona usuarios, técnicos, especialidades, solicitudes, reglas de diagnóstico y demás información necesaria para la operación y control de la plataforma.

## Capacidades principales

Las capacidades principales previstas para Servi Te&Pro son:

* Registro e inicio de sesión de usuarios.
* Gestión de perfiles de clientes y técnicos.
* Registro y gestión de vehículos.
* Registro de especialidades técnicas.
* Gestión de disponibilidad de técnicos.
* Registro de solicitudes de asistencia.
* Registro de la avería y síntomas reportados por el cliente.
* Generación de un diagnóstico preliminar basado en reglas.
* Identificación del tipo de asistencia o especialidad requerida.
* Consulta y gestión de solicitudes por parte de los técnicos.
* Asignación o conexión de una solicitud con un técnico.
* Actualización del estado de la asistencia.
* Registro del diagnóstico o resultado final realizado por el técnico.
* Consulta del historial de solicitudes.
* Administración básica del sistema.

Las funcionalidades adicionales, como cotizaciones, pagos, calificaciones, reseñas, geolocalización avanzada e integraciones externas, serán incorporadas únicamente si se definen dentro del alcance del MVP y de los requerimientos del proyecto.

## Tecnologías

La selección definitiva de tecnologías se establecerá durante la etapa de arquitectura, considerando los requerimientos funcionales y no funcionales del sistema.

De manera preliminar, el proyecto contempla:

* **Frontend:** aplicación web.
* **Backend:** API para la gestión de las funcionalidades del sistema.
* **Base de datos:** sistema de gestión de base de datos relacional.
* **Comunicación:** HTTP/HTTPS y formato JSON.
* **Documentación de API:** OpenAPI.
* **Infraestructura y despliegue:** se evaluará el uso de contenedores y otras herramientas de infraestructura según las necesidades del proyecto.

Las tecnologías específicas se documentarán posteriormente en `05-architecture`.

## Arquitectura

Servi Te&Pro se desarrollará como una aplicación orientada a servicios, con una separación clara entre sus principales responsabilidades funcionales.

La arquitectura definitiva será definida y documentada durante la fase de diseño técnico, teniendo en cuenta el tamaño del proyecto, sus requerimientos, la capacidad del equipo y las necesidades de evolución futuras.

El proyecto no requiere inicialmente la implementación de múltiples microservicios. En caso de que posteriormente se identifique una necesidad técnica que justifique separar determinados componentes, esta decisión deberá ser documentada y sustentada mediante la arquitectura correspondiente.

## Alcance geográfico

La primera versión de Servi Te&Pro estará orientada al departamento del **Huila, Colombia**.

La expansión hacia otros departamentos o regiones no forma parte del alcance inicial y podrá considerarse como una evolución futura del producto.

## Estado actual

**En construcción**

Servi Te&Pro se encuentra actualmente en las fases de análisis del problema, definición de requerimientos, modelado del dominio, diseño de la solución y preparación de la implementación.
