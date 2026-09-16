# Definition of Done (DoD)

> Una Historia de Usuario se considera **DONE** cuando cumple todos los criterios aplicables de esta lista de verificación.
>
> Si falta algún criterio obligatorio aplicable, la historia **NO se considera terminada** y debe permanecer o regresar a **In Progress**.

---

## Lista de verificación obligatoria

### Código

* [ ] El código implementa todos los criterios de aceptación de la Historia de Usuario.
* [ ] El código fue revisado y aprobado por al menos un integrante del equipo mediante un Pull Request (PR).
* [ ] El código cumple los estándares establecidos por el proyecto para formato, linting y calidad.
* [ ] No se introduce deuda técnica sin registrarla en `15-project-control/tech-backlog.md`.
* [ ] El código cumple las convenciones arquitectónicas y de desarrollo definidas para Servi Te&Pro.
* [ ] El código se encuentra registrado en el repositorio oficial del proyecto.

### Pruebas

* [ ] Se escribieron pruebas unitarias para la lógica de negocio nueva o modificada cuando corresponda.
* [ ] La cobertura de pruebas no disminuye respecto a la línea base establecida por el proyecto, cuando exista.
* [ ] Todas las pruebas relevantes se ejecutan correctamente en el entorno disponible.
* [ ] Los criterios de aceptación fueron verificados mediante pruebas automatizadas o manuales.
* [ ] Se verificaron los escenarios relevantes de error y fallo.
* [ ] Las pruebas de integración fueron ejecutadas cuando los cambios afectan la comunicación entre microservicios.

### Integración

* [ ] Los cambios no rompen funcionalidades existentes de Servi Te&Pro.
* [ ] Los cambios no rompen los microservicios o integraciones afectados.
* [ ] Si existen cambios en una API, el contrato OpenAPI correspondiente está actualizado en `07-api/contracts/`.
* [ ] Si existen cambios en el modelo de datos, el `data-model.md` correspondiente está actualizado.
* [ ] Si existen eventos nuevos o modificados, el `event-catalog.md` correspondiente está actualizado.
* [ ] Si un cambio afecta a otro microservicio, su impacto y compatibilidad fueron verificados.
* [ ] Las dependencias entre microservicios afectadas fueron identificadas y verificadas.

### Seguridad

* [ ] Los requisitos de autenticación y autorización fueron verificados cuando corresponda.
* [ ] Los permisos de acceso respetan el rol del usuario y la propiedad de los recursos cuando aplique.
* [ ] No se expone información sensible en el código fuente, logs, respuestas de API o mensajes de error.
* [ ] Las entradas de usuarios y APIs son validadas cuando corresponda.
* [ ] No se incorporan contraseñas, tokens, claves u otros secretos directamente en el código.
* [ ] El cambio no introduce vulnerabilidades de seguridad conocidas.
* [ ] El cambio cumple las reglas definidas en `security-policy.md` y `security-rules.md`.

### Despliegue

* [ ] El código puede integrarse a la rama `dev` sin conflictos pendientes.
* [ ] Las verificaciones de CI/CD son satisfactorias cuando CI/CD esté disponible.
* [ ] La funcionalidad ha sido desplegada en el entorno de staging cuando dicho entorno esté disponible.
* [ ] Se ha ejecutado correctamente una prueba básica de funcionamiento (smoke test) en staging cuando corresponda.

> Durante las primeras etapas del proyecto, algunos criterios de despliegue pueden no ser aplicables porque la infraestructura todavía se encuentra en construcción. Una vez implementada la infraestructura correspondiente, estos criterios serán obligatorios cuando sean aplicables.

### Documentación

* [ ] El `README.md` del microservicio fue actualizado si cambió su interfaz pública, configuración o proceso de ejecución.
* [ ] La documentación OpenAPI fue actualizada si cambió un contrato de API.
* [ ] La documentación del modelo de datos fue actualizada si cambió la estructura de datos.
* [ ] Las reglas de negocio fueron documentadas cuando se introdujeron o modificaron reglas.
* [ ] Si se tomó una decisión técnica o arquitectónica significativa, se creó o actualizó el ADR correspondiente.
* [ ] La documentación relevante del proyecto fue actualizada en el mismo Pull Request cuando corresponda.
* [ ] Los cambios mantienen la trazabilidad con los requisitos y las Historias de Usuario correspondientes.

---

## Excepciones permitidas

Las siguientes excepciones deben ser justificadas y aprobadas por el responsable de coordinación técnica o, si el proyecto es desarrollado por un único integrante, deben quedar registradas y justificadas por el responsable del proyecto:

* Las pruebas E2E pueden omitirse cuando el entorno o la infraestructura necesaria no estén disponibles, siempre que la limitación y el riesgo asociado queden documentados.
* La documentación puede aplazarse excepcionalmente ante una entrega urgente, siempre que el trabajo pendiente sea registrado como deuda técnica.
* La validación en staging puede aplazarse cuando dicho entorno no esté disponible, siempre que se realicen las pruebas posibles en el entorno disponible y se documente la limitación y el riesgo asociado.
* La revisión por un segundo integrante puede no ser posible cuando el proyecto sea desarrollado por un único integrante. En ese caso, debe realizarse una revisión técnica personal antes de integrar el cambio.

Cualquier excepción aprobada debe quedar documentada y no podrá convertirse en un sustituto permanente del criterio correspondiente de la Definition of Done.

---

## Lo que NO constituye un criterio de Done

Los siguientes casos no son suficientes para considerar terminada una Historia de Usuario:

* **"El código está en mi computador."**
  El código debe estar registrado y disponible en el repositorio oficial.

* **"Funciona en mi entorno local."**
  Debe verificarse en el entorno disponible y, cuando exista, en staging.

* **"El Pull Request fue creado."**
  La creación del PR no significa que la revisión y las verificaciones requeridas hayan finalizado.

* **"El código fue escrito."**
  La implementación por sí sola no demuestra el cumplimiento de los criterios de aceptación.

* **"El PM/PO o instructor lo aprobó."**
  La aprobación funcional no reemplaza los criterios técnicos de la Definition of Done.

* **"No encontré errores manualmente."**
  Las pruebas requeridas deben ejecutarse y registrarse.

* **"La documentación puede hacerse después."**
  La documentación aplicable forma parte del trabajo terminado.

---

## Regla final

Una Historia de Usuario solo puede trasladarse a **Done** cuando el equipo pueda demostrar que:

1. La funcionalidad solicitada fue implementada.
2. Todos los criterios de aceptación fueron satisfechos.
3. Las pruebas requeridas fueron ejecutadas correctamente.
4. Los cambios fueron revisados.
5. Las integraciones afectadas fueron verificadas.
6. Los requisitos de seguridad aplicables fueron satisfechos.
7. La documentación requerida fue actualizada.
8. La deuda técnica pendiente fue registrada correctamente.
9. El cambio se encuentra disponible en el repositorio oficial.
10. No existen bloqueos conocidos que impidan considerar terminado el trabajo.

---

## Aplicación de la Definition of Done

La Definition of Done se aplica a todas las Historias de Usuario y trabajos que se declaren completados dentro de Servi Te&Pro.

Los criterios se evaluarán según su **aplicabilidad al trabajo realizado**. No se debe marcar como incumplido un criterio que técnicamente no corresponda a la Historia de Usuario.

Por ejemplo:

* Una HU que no modifica una API no necesita actualizar un contrato OpenAPI.
* Una HU que no modifica datos no necesita actualizar el modelo de datos.
* Una HU que no modifica eventos no necesita actualizar el catálogo de eventos.
* Una HU que no requiere autenticación no necesita implementar mecanismos de autenticación adicionales.

La Definition of Done establece el estándar mínimo de calidad, pero no exige actividades que no sean relevantes para el cambio realizado.

---

## Documentos relacionados

* Definition of Ready → `00-governance/definition-of-ready.md`
* Agile Team Conventions → `00-governance/agile-conventions.md`
* Git Conventions → `00-governance/git-conventions.md`
* Documentation Rules → `00-governance/documentation-rules.md`
* Microservices Documentation → `00-governance/microservices-documentation.md`
* Security Policy → `00-governance/security-policy.md`
* Security Rules → `00-governance/security-rules.md`
* Technical Debt Backlog → `15-project-control/tech-backlog.md`
* User Stories → `04-requirements/user-stories.md`
* Architecture → `05-architecture/`
* Data → `06-data/`
* API Contracts → `07-api/contracts/`
