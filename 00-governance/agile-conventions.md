# Agile Team Conventions

> Define cómo trabaja el equipo de Servi Te&Pro durante sus ciclos de desarrollo. Estas convenciones establecen la forma de planificar, ejecutar, revisar y mejorar el trabajo del proyecto.
>
> Debido a que Servi Te&Pro es un proyecto basado en microservicios y requiere investigación, aprendizaje técnico, documentación y desarrollo incremental, la planificación se adapta progresivamente a la capacidad real del equipo y al avance del proyecto.

---

## 1. Equipo y capacidad de trabajo

| Campo                       | Definición                                            |
| --------------------------- | ----------------------------------------------------- |
| Equipo actual               | 2 integrantes                                         |
| Dedicación semanal          | 8–10 horas aproximadamente                            |
| Modalidad de trabajo        | Colaborativa y remota/presencial según disponibilidad |
| Inicio del proyecto         | 1 de septiembre de 2026                               |
| Fecha estimada de entrega   | Abril de 2027                                         |
| Herramientas de gestión     | Trello + GitHub                                       |
| Herramienta de comunicación | Discord                                               |
| Metodología                 | Agile con Sprints de 2 semanas                        |

> La capacidad de trabajo podrá ajustarse si cambia el número de integrantes o la disponibilidad del equipo. La velocidad del equipo no se utilizará como métrica de desempeño individual.

---

## 2. Estructura del Sprint

Los Sprints tendrán una duración estándar de **2 semanas**, con planificación y cierre de lunes a viernes.

Cada Sprint debe producir un incremento verificable del proyecto. El incremento puede corresponder a funcionalidad implementada, documentación técnica validada, infraestructura, pruebas o una combinación de estos elementos, siempre que represente un avance concreto y demostrable.

### Sprint 0 — Preparación

El proyecto utilizará un **Sprint 0** para establecer las bases necesarias antes de iniciar el desarrollo funcional.

El Sprint 0 contempla:

* Organización del repositorio.
* Definición de las reglas de gobernanza.
* Estructuración de la documentación.
* Definición del problema y contexto.
* Análisis del dominio.
* Definición inicial del producto.
* Elaboración y revisión de requisitos.
* Definición inicial de la arquitectura de microservicios.
* Definición inicial de los modelos y responsabilidades de datos.
* Configuración de las herramientas de trabajo.
* Preparación del backlog inicial.

El Sprint 0 no se considera un Sprint de desarrollo funcional, sino una etapa de preparación y alineación del proyecto.

### Sprints de desarrollo

A partir del Sprint 1 se iniciará el desarrollo incremental de Servi Te&Pro.

| Campo                 | Valor                                                  |
| --------------------- | ------------------------------------------------------ |
| Duración              | 2 semanas                                              |
| Inicio habitual       | Lunes                                                  |
| Finalización habitual | Viernes de la segunda semana                           |
| Planificación         | Primer día del Sprint                                  |
| Daily                 | Durante los días de trabajo                            |
| Review                | Último día del Sprint                                  |
| Retrospectiva         | Después de la Review                                   |
| Refinamiento          | Durante el Sprint, antes de la siguiente planificación |

La planificación detallada de cada Sprint se realizará progresivamente mediante el Backlog Refinement.

---

## 3. Planificación general

El proyecto comenzó el **1 de septiembre de 2026** y tiene como fecha estimada de entrega **abril de 2027**.

Debido a que el desarrollo de Servi Te&Pro involucra aprendizaje, investigación y decisiones arquitectónicas que pueden modificar el alcance técnico, no se establecerá desde el inicio una asignación definitiva de todas las historias de usuario hasta abril.

Se trabajará con una planificación progresiva:

1. Definir los objetivos generales del proyecto.
2. Refinar las historias de usuario.
3. Priorizar las funcionalidades.
4. Seleccionar el trabajo del siguiente Sprint.
5. Ejecutar y validar el incremento.
6. Revisar los resultados.
7. Ajustar la planificación de los siguientes Sprints.

La planificación podrá modificarse cuando aparezcan nuevas dependencias, riesgos, decisiones arquitectónicas o necesidades identificadas durante el desarrollo.

---

## 4. Objetivo de cada Sprint

Cada Sprint debe tener un objetivo claro denominado **Sprint Goal**.

El Sprint Goal debe:

* Estar relacionado con el alcance de Servi Te&Pro.
* Ser alcanzable con la capacidad disponible.
* Estar relacionado con una necesidad funcional, técnica o arquitectónica.
* Permitir verificar un resultado concreto al finalizar el Sprint.
* Servir como criterio para priorizar el trabajo durante el Sprint.

Ejemplos de objetivos posibles:

* Establecer la estructura base de un microservicio.
* Implementar el flujo inicial de autenticación.
* Implementar la gestión de clientes.
* Implementar la creación de solicitudes de servicio.
* Implementar la gestión de técnicos.
* Implementar la comunicación entre determinados microservicios.
* Implementar persistencia y migraciones.
* Incorporar pruebas de integración.
* Fortalecer la seguridad de los servicios.
* Integrar el flujo principal de extremo a extremo.

Estos ejemplos no constituyen una asignación definitiva de funcionalidades a los Sprints.

---

## 5. Ceremonias

### Sprint Planning

* **Cuándo:** Primer día del Sprint.
* **Duración:** Máximo 1 hora.
* **Quiénes:** Todo el equipo.
* **Objetivo:** Definir el Sprint Goal, seleccionar las historias de usuario y tareas que se desarrollarán durante el Sprint y establecer el Sprint Backlog.
* **Herramientas:** Trello y GitHub.

Durante la planificación se debe:

1. Revisar el objetivo del proyecto.
2. Revisar las historias disponibles en el Backlog.
3. Confirmar que las historias seleccionadas cumplen la Definition of Ready.
4. Revisar las dependencias conocidas.
5. Estimar las historias cuando sea necesario.
6. Definir el Sprint Goal.
7. Seleccionar las historias que puedan completarse con la capacidad disponible.
8. Dividir las historias en tareas técnicas cuando sea necesario.

**Resultado:** Sprint Backlog actualizado y Sprint Goal definido.

---

### Daily Stand-up

* **Cuándo:** Durante los días de trabajo del Sprint.
* **Duración:** Máximo 15 minutos.
* **Quiénes:** Todo el equipo.
* **Herramienta:** Discord, cuando la reunión sea remota.

Cada integrante responde:

1. ¿Qué hice desde la última Daily?
2. ¿Qué voy a realizar a continuación?
3. ¿Tengo algún bloqueo o dependencia?

Las discusiones técnicas que requieran más tiempo deben realizarse posteriormente con los integrantes involucrados.

La Daily no debe convertirse en una reunión extensa de resolución técnica.

---

### Sprint Review

* **Cuándo:** Último día del Sprint.
* **Duración:** Máximo 30 minutos.
* **Quiénes:** Equipo + instructor/Product Owner cuando corresponda.
* **Objetivo:** Revisar el incremento producido durante el Sprint, demostrar los resultados y recopilar retroalimentación.

Durante la Review se debe presentar:

* Sprint Goal.
* Historias completadas.
* Funcionalidad implementada.
* Documentación actualizada.
* Pruebas realizadas.
* Problemas encontrados.
* Trabajo pendiente, cuando corresponda.

Solo se considerará completado el trabajo que cumpla la **Definition of Done**.

---

### Sprint Retrospective

* **Cuándo:** Último día del Sprint, después de la Review.
* **Duración:** Máximo 30–45 minutos.
* **Quiénes:** Todo el equipo.

La retrospectiva analizará:

* Qué funcionó correctamente.
* Qué problemas se presentaron.
* Qué puede mejorarse.
* Qué decisiones deben cambiarse.
* Qué acciones se realizarán en el siguiente Sprint.

Cada retrospectiva debe generar al menos **una acción de mejora**, indicando:

* Acción.
* Responsable.
* Fecha o Sprint de seguimiento.

---

### Backlog Refinement

* **Cuándo:** Durante el Sprint, preferiblemente antes de la siguiente planificación.
* **Duración:** Máximo 1 hora.
* **Quiénes:** Todo el equipo.
* **Herramientas:** Trello y GitHub.

Durante el Refinement se deben:

* Revisar historias futuras.
* Aclarar criterios de aceptación.
* Identificar dependencias.
* Identificar riesgos.
* Identificar necesidades de datos.
* Identificar necesidades de seguridad.
* Revisar dependencias entre microservicios.
* Revisar impactos arquitectónicos.
* Estimar las historias cuando sea necesario.
* Dividir historias demasiado grandes.

Una historia estará preparada para ingresar a un Sprint cuando cumpla la **Definition of Ready**.

---

## 6. Estimación

### Escala de Story Points

| Puntos | Significado                                                                                     |
| ------ | ----------------------------------------------------------------------------------------------- |
| 1      | Trivial — trabajo pequeño y de baja incertidumbre                                               |
| 2      | Pequeño — puede completarse aproximadamente en un día de trabajo                                |
| 3      | Mediano — requiere análisis y desarrollo moderado                                               |
| 5      | Grande — requiere una parte importante del Sprint                                               |
| 8      | Muy grande — presenta una complejidad o incertidumbre considerable y debe evaluarse su división |
| 13     | Demasiado grande — DEBE dividirse antes de ingresar al Sprint                                   |

Los Story Points representan una combinación de:

* Complejidad.
* Esfuerzo.
* Incertidumbre.
* Dependencias.
* Riesgo técnico.

Los Story Points **no representan una cantidad fija de horas**.

### Técnica de estimación

Inicialmente se utilizará **Planning Poker**, cuando el tamaño o complejidad de las historias requiera una estimación conjunta.

Cuando una historia sea claramente pequeña y no exista incertidumbre significativa, el equipo podrá realizar una estimación directa.

### Reglas

* Una historia estimada en 13 puntos DEBE dividirse.
* Una historia estimada en 8 puntos DEBERÍA revisarse para determinar si puede dividirse.
* Si existen diferencias importantes entre las estimaciones, se deben discutir las razones antes de volver a estimar.
* Las estimaciones podrán actualizarse cuando aparezca información nueva que cambie significativamente la complejidad de la historia.

---

## 7. Capacidad del Sprint

La capacidad inicial estimada será de:

**8–10 horas de trabajo por semana.**

Por lo tanto, un Sprint de dos semanas tendrá una capacidad aproximada de:

**16–20 horas de trabajo.**

Esta capacidad incluye:

* Análisis.
* Investigación.
* Diseño.
* Programación.
* Pruebas.
* Documentación.
* Revisión de código.
* Corrección de errores.
* Reuniones Agile.
* Actividades relacionadas con la arquitectura.

Durante los primeros Sprints no se establecerá una cantidad fija de Story Points como capacidad.

La capacidad se ajustará después de observar el comportamiento real del equipo.

---

## 8. Velocidad del equipo

La velocidad se calculará utilizando los Story Points de las historias que hayan cumplido completamente la Definition of Done al finalizar cada Sprint.

| Sprint   | Story Points completados | Observaciones |
| -------- | -----------------------: | ------------- |
| Sprint 1 |                        — | —             |
| Sprint 2 |                        — | —             |
| Sprint 3 |                        — | —             |
| Promedio |                        — | —             |

Después de los primeros Sprints se podrá calcular una velocidad promedio para mejorar la planificación.

La velocidad será utilizada únicamente como herramienta de planificación y **no como indicador de rendimiento individual**.

---

## 9. Herramientas de trabajo

### Trello

Trello será utilizado principalmente para:

* Visualizar el Backlog.
* Organizar las historias de usuario.
* Planificar el Sprint.
* Dividir historias en tareas.
* Visualizar el estado del trabajo.

### GitHub

GitHub será utilizado como plataforma principal para:

* Repositorio de código.
* Documentación técnica.
* Ramas.
* Commits.
* Pull Requests.
* Issues, cuando corresponda.
* Control de versiones.

### Discord

Discord será utilizado para:

* Comunicación del equipo.
* Daily cuando sea necesario.
* Reuniones.
* Coordinación rápida.
* Discusiones técnicas iniciales.

Las decisiones técnicas relevantes no deben quedar únicamente en Discord. Deben trasladarse a la documentación correspondiente o registrarse mediante un ADR cuando corresponda.

---

## 10. Tablero del Backlog

El tablero de trabajo utilizará las siguientes columnas:

| Columna     | Significado                                                            |
| ----------- | ---------------------------------------------------------------------- |
| Backlog     | Historias y tareas pendientes de priorización o refinamiento           |
| Ready       | Historias que cumplen la Definition of Ready                           |
| In Progress | Trabajo actualmente en desarrollo                                      |
| In Review   | Trabajo pendiente de revisión mediante Pull Request o revisión técnica |
| Done        | Trabajo que cumple completamente la Definition of Done                 |

El trabajo debe desplazarse entre columnas de acuerdo con su estado real.

Una historia no debe pasar a **Done** únicamente porque el código haya sido escrito.

---

## 11. Reglas específicas para Servi Te&Pro

Debido a que Servi Te&Pro utiliza una arquitectura basada en microservicios, las siguientes reglas son obligatorias:

* Las historias de usuario deben estar relacionadas con el alcance definido del sistema.
* Las funcionalidades deben respetar los roles definidos: **Cliente, Técnico y Administrador**.
* Cada microservicio debe mantener responsabilidades claramente delimitadas.
* Los cambios en contratos de API deben documentarse.
* Los cambios en modelos de datos deben documentarse.
* Los cambios en eventos deben documentarse cuando formen parte de la arquitectura.
* Los cambios de seguridad deben actualizar la documentación correspondiente.
* Los cambios arquitectónicos relevantes deben registrarse mediante un ADR.
* Las dependencias entre microservicios deben identificarse antes de comenzar el desarrollo cuando sean conocidas.
* Una historia no puede considerarse Done si no cumple la Definition of Done.
* Los bloqueos deben comunicarse oportunamente.
* La documentación debe actualizarse junto con los cambios que la afecten.
* Las decisiones tomadas durante el desarrollo deben conservar trazabilidad.
* El aprendizaje técnico que implique una decisión relevante debe reflejarse en la documentación cuando afecte el diseño o funcionamiento del sistema.

---

## 12. Incremento del Sprint

Al finalizar cada Sprint debe existir un resultado verificable.

Dependiendo del Sprint, el incremento puede incluir:

* Código funcional.
* Microservicios implementados.
* Endpoints funcionales.
* Persistencia de datos.
* Integración entre servicios.
* Pruebas automatizadas.
* Pruebas de integración.
* Documentación técnica.
* Diagramas actualizados.
* Configuración de infraestructura.
* Correcciones de errores.
* Mejoras de seguridad.

El incremento debe poder ser revisado por el equipo y, cuando corresponda, presentado al instructor.

---

## 13. Gestión del aprendizaje y la incertidumbre

Servi Te&Pro es también un proyecto de aprendizaje técnico. Por esta razón, pueden aparecer durante el desarrollo tecnologías, conceptos, problemas o decisiones que no hayan sido completamente definidos durante la planificación inicial.

Cuando esto ocurra:

1. Se identifica el problema o necesidad de aprendizaje.
2. Se determina si afecta el Sprint actual.
3. Se realiza la investigación necesaria.
4. Se documentan las conclusiones relevantes.
5. Se actualiza la arquitectura, requisitos o documentación si corresponde.
6. Se crea una tarea técnica o historia cuando el trabajo requerido sea significativo.
7. Se incorpora al Backlog cualquier trabajo que no pueda completarse dentro del Sprint actual.

El aprendizaje no debe utilizarse como justificación para introducir cambios sin control en el alcance del proyecto.

---

## 14. Gestión de cambios durante el Sprint

Una vez iniciado un Sprint, se debe evitar incorporar trabajo adicional que comprometa el Sprint Goal.

Si aparece una necesidad urgente:

1. Se analiza su importancia.
2. Se determina su impacto.
3. Se revisa la capacidad disponible.
4. Se decide si puede incorporarse sin comprometer el Sprint Goal.
5. Si no puede incorporarse, se registra en el Backlog para su priorización posterior.

Los cambios que afecten significativamente la arquitectura deben seguir las reglas de gobernanza y ADR correspondientes.

---

## 15. Reglas para un proyecto con capacidad reducida

Debido a que el equipo actualmente está compuesto por dos integrantes y existe la posibilidad de que el proyecto continúe siendo desarrollado por un solo integrante, la planificación deberá adaptarse a la capacidad real disponible.

Si el equipo pasa a estar compuesto por un solo integrante:

* Se mantendrá la estructura Agile mientras resulte útil.
* Se reducirá el alcance del Sprint cuando sea necesario.
* Se priorizarán historias de mayor valor para el proyecto.
* Se evitará comprometer una cantidad de trabajo superior a la capacidad disponible.
* Se mantendrán las prácticas de revisión y documentación necesarias para garantizar la calidad.
* Las decisiones técnicas importantes deberán continuar siendo documentadas.

La cantidad de trabajo comprometida en un Sprint dependerá de la capacidad real y no del número esperado de funcionalidades.

---

## 16. Documentos relacionados

* Definition of Ready → `00-governance/definition-of-ready.md`
* Definition of Done → `00-governance/definition-of-done.md`
* Git Conventions → `00-governance/git-conventions.md`
* Documentation Rules → `00-governance/documentation-rules.md`
* Microservices Documentation → `00-governance/microservices-documentation.md`
* Security Policy → `00-governance/security-policy.md`
* Security Rules → `00-governance/security-rules.md`
* Gestión de riesgos → `15-project-control/risks.md`
* Backlog de deuda técnica → `15-project-control/tech-backlog.md`
* Historias de usuario → `04-requirements/user-stories.md`
* Arquitectura → `05-architecture/`
* Datos → `06-data/`

---

## 17. Revisión de estas convenciones

Estas convenciones deben revisarse periódicamente durante las retrospectivas.

Cualquier cambio debe:

1. Ser discutido por el equipo.
2. Tener una justificación.
3. Evaluar su impacto.
4. Actualizar este documento cuando corresponda.
5. Registrarse mediante un ADR si representa una decisión técnica o arquitectónica significativa.
6. Comunicarse antes de aplicarse como una nueva regla de trabajo.

Las convenciones Agile son parte de la gobernanza del proyecto y deben mantenerse sincronizadas con la forma real de trabajo de Servi Te&Pro.
