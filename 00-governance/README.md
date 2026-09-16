# 00-gobernanza — Reglas del Equipo

> Esta sección define los acuerdos y reglas que el equipo de Servi Te&Pro se compromete a seguir durante todo el proyecto.
> Cada integrante del equipo debe leer y comprender todos los documentos de esta sección antes de realizar su primer commit.

---

## Documentos de esta sección

| Archivo                                                            | Propósito                                                                                                                      |
| ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| [git-conventions.md](./git-conventions.md)                         | Estrategia de ramas, formato de commits, política de Pull Requests y reglas de integración                                     |
| [agile-conventions.md](./agile-conventions.md)                     | Estructura de los sprints, ceremonias, estimación y gestión del backlog                                                        |
| [definition-of-done.md](./definition-of-done.md)                   | Lista de verificación que debe cumplir cada historia de usuario para considerarse terminada                                    |
| [definition-of-ready.md](./definition-of-ready.md)                 | Lista de verificación que debe cumplir una historia de usuario antes de ingresar a un sprint                                   |
| [documentation-rules.md](./documentation-rules.md)                 | Reglas para crear, actualizar, organizar y eliminar la documentación del proyecto                                              |
| [microservices-documentation.md](./microservices-documentation.md) | Documentación y estándares requeridos para cada microservicio                                                                  |
| [security-policy.md](./security-policy.md)                         | Política del equipo para gestionar vulnerabilidades, riesgos de seguridad e incidentes de seguridad                            |
| [security-rules.md](./security-rules.md)                           | Reglas de seguridad a nivel de código para autenticación, autorización, secretos, validación de entradas y protección de datos |

---

## Aplicación de la gobernanza

Las reglas de gobernanza se aplican a **todo el proyecto Servi Te&Pro**, incluyendo todas las secciones del proyecto, microservicios, documentación, código fuente y miembros del equipo.

Estas reglas establecen los estándares mínimos que el equipo debe seguir durante las etapas de análisis, diseño, desarrollo, pruebas, integración y despliegue.

Si una regla de gobernanza entra en conflicto con una convención local, prevalece la regla de gobernanza, a menos que el equipo apruebe explícitamente un cambio y lo registre mediante un Architecture Decision Record (ADR).

> Las reglas de gobernanza no deben modificarse de manera individual.
> Cualquier cambio requiere el acuerdo del equipo, debe documentarse indicando su motivo y debe comunicarse antes del siguiente sprint.

---

## Principios de gobernanza

El equipo de Servi Te&Pro sigue los siguientes principios:

* **Consistencia:** Los mismos estándares del proyecto se aplican en todos los microservicios y secciones del proyecto.
* **Trazabilidad:** Las decisiones técnicas, funcionales y organizacionales importantes deben quedar documentadas.
* **Calidad:** El código y la documentación deben cumplir los criterios de calidad acordados por el proyecto antes de considerarse terminados.
* **Seguridad:** Los requisitos de seguridad deben considerarse durante todo el ciclo de vida del desarrollo, no únicamente al final.
* **Colaboración:** Los cambios que afecten las reglas del equipo o los estándares del proyecto requieren el acuerdo de sus integrantes.
* **Transparencia:** Los riesgos, la deuda técnica, los bloqueos y las desviaciones relevantes deben documentarse y comunicarse.
* **Mejora continua:** Las reglas de gobernanza pueden evolucionar cuando el equipo identifique una mejora justificada.

---

## Proceso para cambiar la gobernanza

Un cambio en una regla de gobernanza debe seguir los siguientes pasos:

1. Identificar la regla que necesita ser modificada.
2. Explicar el motivo y el impacto esperado del cambio.
3. Discutir el cambio con el equipo.
4. Llegar a un acuerdo entre los integrantes.
5. Actualizar el documento de gobernanza correspondiente.
6. Crear o actualizar un ADR cuando el cambio represente una decisión arquitectónica o técnica significativa.
7. Comunicar el cambio a todos los integrantes del equipo antes del siguiente sprint.

---

## Responsabilidad del equipo

Cada integrante del equipo es responsable de:

* Leer y comprender los documentos de gobernanza.
* Seguir las convenciones acordadas para el proyecto.
* Informar conflictos, ambigüedades o reglas que hayan quedado desactualizadas.
* Actualizar la documentación cuando sus cambios lo requieran.
* Respetar los estándares de Git, Agile, documentación, seguridad y microservicios establecidos por el proyecto.

La sección de gobernanza es una **parte viva de la documentación del proyecto** y debe mantenerse sincronizada con la forma real en que trabaja el equipo de Servi Te&Pro.
