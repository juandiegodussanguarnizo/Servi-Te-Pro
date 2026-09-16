# Definition of Ready (DoR)

> Una Historia de Usuario se considera **Ready** cuando el equipo de Servi Te&Pro dispone de la información necesaria para comenzar su desarrollo en el siguiente Sprint sin tener que resolver preguntas fundamentales durante su ejecución.
>
> Si una Historia de Usuario no cumple los criterios aplicables de esta Definition of Ready, debe regresar al proceso de refinamiento antes de ser seleccionada para un Sprint.

---

## 1. Lista de verificación de la Definition of Ready

Antes de mover una Historia de Usuario a **Ready**, el equipo debe verificar los siguientes criterios.

### Claridad

* [ ] La Historia de Usuario está escrita utilizando el formato: **Como [rol], quiero [acción], para [beneficio]**.
* [ ] El rol corresponde a uno de los roles definidos para Servi Te&Pro: **Cliente, Técnico o Administrador**.
* [ ] El beneficio esperado es claro y verificable.
* [ ] El alcance de la Historia de Usuario está claramente definido.
* [ ] La Historia de Usuario describe una necesidad concreta.
* [ ] La Historia de Usuario no incluye funcionalidades que no estén relacionadas con su objetivo.
* [ ] La Historia de Usuario puede ser entendida por los integrantes involucrados sin interpretaciones fundamentales diferentes.

---

## 2. Criterios de aceptación

* [ ] La Historia de Usuario tiene criterios de aceptación claramente definidos.
* [ ] Los criterios de aceptación utilizan, cuando corresponda, el formato **Given / When / Then**.
* [ ] Los criterios cubren el flujo principal o caso exitoso.
* [ ] Los criterios cubren los principales escenarios de error.
* [ ] Los criterios pueden verificarse mediante pruebas automatizadas o manuales.
* [ ] No existen criterios ambiguos o subjetivos.
* [ ] El comportamiento esperado para entradas válidas está definido.
* [ ] El comportamiento esperado para entradas inválidas está definido cuando corresponda.
* [ ] El resultado esperado o estado final del sistema está claramente definido.
* [ ] Los criterios de aceptación permiten determinar objetivamente cuándo la Historia de Usuario cumple su objetivo.

---

## 3. Dependencias

* [ ] Se identificaron las dependencias relevantes de la Historia de Usuario.
* [ ] Se identificaron las dependencias con otros microservicios cuando corresponda.
* [ ] Se identificaron las dependencias con APIs, datos, infraestructura o servicios externos.
* [ ] Las dependencias que bloquean el desarrollo están resueltas o cuentan con una solución previamente definida.
* [ ] Si la Historia de Usuario depende de otra Historia de Usuario, dicha dependencia está completada o proporciona los elementos necesarios para comenzar.
* [ ] Se identificaron las integraciones externas necesarias.
* [ ] Se conoce quién es responsable de resolver cada dependencia que pueda bloquear el trabajo.
* [ ] Las dependencias críticas no representan un bloqueo desconocido para el Sprint.

---

## 4. Estimación

* [ ] La Historia de Usuario fue estimada utilizando la técnica definida en `agile-conventions.md`.
* [ ] El equipo tiene suficiente información para realizar una estimación razonable.
* [ ] Existe acuerdo sobre la estimación realizada.
* [ ] La Historia de Usuario puede completarse dentro de un Sprint.
* [ ] Si la Historia de Usuario es demasiado grande, fue dividida en historias más pequeñas.
* [ ] Una Historia de Usuario estimada en **13 Story Points DEBE dividirse** antes de ingresar a un Sprint.
* [ ] Una Historia de Usuario estimada en **8 Story Points DEBERÍA revisarse** para determinar si puede dividirse.
* [ ] La Historia de Usuario no supera el tamaño máximo establecido por las convenciones Agile del proyecto.

---

## 5. Preparación técnica

Antes de comenzar el desarrollo, se debe verificar que la información y los recursos técnicos necesarios estén disponibles.

* [ ] Los accesos necesarios están disponibles.
* [ ] Los repositorios necesarios están disponibles.
* [ ] Los ambientes necesarios están disponibles o existe una alternativa documentada.
* [ ] Las herramientas necesarias para desarrollar y probar la funcionalidad están disponibles.
* [ ] Si la Historia de Usuario requiere una nueva API o modifica una existente, el contrato OpenAPI correspondiente está definido.
* [ ] Si la Historia de Usuario requiere cambios en la base de datos, el modelo de datos está definido.
* [ ] Se identificó el impacto sobre otros microservicios.
* [ ] Se identificaron las restricciones técnicas conocidas.
* [ ] Se identificaron las necesidades de configuración necesarias para implementar la Historia de Usuario.
* [ ] Las decisiones arquitectónicas relevantes fueron identificadas.
* [ ] Las decisiones arquitectónicas que requieren registro fueron documentadas mediante un ADR.

---

## 6. Requisitos no funcionales

Los requisitos no funcionales aplicables deben identificarse antes de iniciar el desarrollo.

* [ ] Se identificaron los requisitos de rendimiento cuando sean aplicables.
* [ ] Se identificaron los requisitos de seguridad cuando sean aplicables.
* [ ] Se consideraron autenticación y autorización cuando correspondan.
* [ ] Se consideró la validación de entradas cuando corresponda.
* [ ] Se consideró la protección de datos cuando corresponda.
* [ ] Se consideraron los requisitos de observabilidad cuando sean aplicables.
* [ ] Se identificaron las necesidades de logs, métricas o trazas cuando correspondan.
* [ ] Se identificaron otros requisitos no funcionales aplicables, como disponibilidad, confiabilidad, mantenibilidad o escalabilidad.

---

## 7. Reglas de negocio

Cuando la Historia de Usuario implique reglas de negocio:

* [ ] Las reglas de negocio necesarias están identificadas.
* [ ] Las reglas de negocio están claramente definidas.
* [ ] No existen contradicciones conocidas entre las reglas de negocio y los requisitos.
* [ ] Las reglas que deben implementarse están asociadas con los criterios de aceptación.
* [ ] Las reglas nuevas o modificadas están identificadas para su posterior documentación.

---

## 8. Datos

Cuando la Historia de Usuario requiera trabajar con datos:

* [ ] Las entidades o estructuras de datos involucradas están identificadas.
* [ ] Se conoce qué microservicio es responsable de los datos.
* [ ] Se identificaron las operaciones necesarias sobre los datos.
* [ ] Se identificaron las validaciones necesarias.
* [ ] Se identificaron las relaciones o dependencias relevantes.
* [ ] Los cambios requeridos al modelo de datos están definidos.
* [ ] Las migraciones necesarias fueron identificadas cuando correspondan.
* [ ] Se consideraron las restricciones de integridad y protección de datos aplicables.

---

## 9. Arquitectura y microservicios

Debido a que Servi Te&Pro utiliza una arquitectura basada en microservicios, cada Historia de Usuario debe considerar su impacto arquitectónico.

* [ ] Se identificó qué microservicio o microservicios están involucrados.
* [ ] La responsabilidad de cada microservicio involucrado está clara.
* [ ] Se identificaron las comunicaciones necesarias entre microservicios.
* [ ] Se identificaron los contratos de API afectados cuando corresponda.
* [ ] Se identificaron los eventos involucrados cuando corresponda.
* [ ] Se identificaron las dependencias entre servicios.
* [ ] Se verificó que la solución propuesta respete las responsabilidades definidas para cada microservicio.
* [ ] Se identificó si la Historia de Usuario requiere modificar una decisión arquitectónica existente.
* [ ] Las decisiones arquitectónicas relevantes fueron documentadas cuando corresponda.

---

## 10. Trazabilidad

Antes de considerar una Historia de Usuario como Ready:

* [ ] La Historia de Usuario está relacionada con uno o más requisitos cuando corresponda.
* [ ] Los criterios de aceptación están relacionados con el objetivo de la Historia de Usuario.
* [ ] Las reglas de negocio aplicables están identificadas.
* [ ] Los componentes o microservicios afectados están identificados.
* [ ] Las necesidades de datos están identificadas cuando corresponda.
* [ ] Las necesidades de seguridad están identificadas cuando corresponda.
* [ ] Las dependencias técnicas y funcionales relevantes están identificadas.

La trazabilidad debe permitir responder:

> **¿Qué requisito origina esta Historia de Usuario, qué parte del sistema afecta y cómo se verificará su cumplimiento?**

---

## 11. Criterio final de Ready

Una Historia de Usuario puede trasladarse a **Ready** cuando el equipo pueda responder afirmativamente a las siguientes preguntas:

1. ¿Entendemos qué necesita el usuario?
2. ¿Sabemos qué funcionalidad debe construirse?
3. ¿Sabemos cómo determinar si la funcionalidad cumple su objetivo?
4. ¿Conocemos las principales reglas de negocio?
5. ¿Conocemos las dependencias?
6. ¿Conocemos los microservicios afectados?
7. ¿Conocemos los cambios de datos necesarios?
8. ¿Conocemos los requisitos de seguridad aplicables?
9. ¿Podemos estimar razonablemente el trabajo?
10. ¿Podemos completar la Historia de Usuario dentro de un Sprint?
11. ¿Tenemos los recursos necesarios para comenzar?
12. ¿No existen preguntas fundamentales pendientes que bloqueen el desarrollo?

Si alguna de estas preguntas tiene una respuesta negativa que pueda impedir el inicio del trabajo, la Historia de Usuario debe regresar a **Refinement**.

---

## 12. Razones comunes por las que una Historia de Usuario NO está Ready

| Problema                                  | Acción requerida                                                                 |
| ----------------------------------------- | -------------------------------------------------------------------------------- |
| Requisitos poco claros                    | Realizar una sesión de refinamiento con los responsables correspondientes        |
| Beneficio desconocido                     | Definir claramente el objetivo y valor de la Historia de Usuario                 |
| Criterios de aceptación incompletos       | Definir los criterios antes de incluir la historia en un Sprint                  |
| Dependencias desconocidas                 | Identificar y documentar las dependencias                                        |
| Dependencia bloqueante                    | Resolverla o definir una solución viable antes de comenzar                       |
| Historia demasiado grande                 | Dividirla en historias más pequeñas                                              |
| Falta de estimación                       | Refinar la historia y realizar la estimación                                     |
| Falta de acceso                           | Obtener el acceso requerido o documentar una alternativa aprobada                |
| Ambiente inexistente                      | Preparar el ambiente o establecer una alternativa temporal                       |
| API no definida                           | Definir el contrato y actualizar OpenAPI                                         |
| Modelo de datos indefinido                | Definir el modelo antes de implementar cambios de persistencia                   |
| Impacto desconocido en otro microservicio | Analizar la integración y definir los cambios requeridos                         |
| Requisitos de seguridad desconocidos      | Definir autenticación, autorización, validación y protección de datos aplicables |
| Decisión arquitectónica pendiente         | Resolverla y documentarla mediante ADR cuando corresponda                        |
| Regla de negocio ambigua                  | Aclarar la regla antes de iniciar el desarrollo                                  |

---

## 13. DoR vs DoD

|                           | Definition of Ready (DoR)                                            | Definition of Done (DoD)                                             |
| ------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Cuándo**                | Antes de iniciar la Historia de Usuario                              | Después de completar el trabajo                                      |
| **Propósito**             | Garantizar que la historia puede comenzar sin bloqueos fundamentales | Garantizar que el trabajo cumple los estándares de calidad y entrega |
| **Pregunta principal**    | ¿Podemos empezar?                                                    | ¿Realmente terminamos?                                               |
| **Momento de aplicación** | Refinement / Sprint Planning                                         | Desarrollo / Review                                                  |
| **Resultado**             | La HU puede pasar a `Ready`                                          | La HU puede pasar a `Done`                                           |

---

## 14. Relación con el proceso Agile

El flujo esperado para una Historia de Usuario es:

```text
Backlog
   ↓
Refinement
   ↓
Definition of Ready
   ↓
Ready
   ↓
Sprint Planning
   ↓
In Progress
   ↓
In Review
   ↓
Definition of Done
   ↓
Done
```

La **Definition of Ready** controla las condiciones necesarias para comenzar.

La **Definition of Done** controla las condiciones necesarias para terminar.

Ninguna de las dos debe utilizarse como sustituto de las actividades de análisis, desarrollo, pruebas o documentación.

---

## 15. Aplicación progresiva

Durante las primeras etapas del proyecto pueden existir elementos técnicos que todavía estén en construcción, como:

* Infraestructura de despliegue.
* CI/CD.
* Ambientes de staging.
* Automatización de pruebas.
* Observabilidad.
* Integraciones entre microservicios.

En estos casos, la Historia de Usuario no debe considerarse Ready si la ausencia del elemento constituye un bloqueo para su desarrollo.

Cuando el elemento no sea necesario para iniciar la Historia de Usuario, podrá quedar como una actividad futura dentro del Backlog.

La aplicación de la DoR debe adaptarse al estado real del proyecto sin eliminar los criterios necesarios para garantizar una planificación adecuada.

---

## 16. Responsabilidad

Todos los integrantes del equipo son responsables de participar en la validación de la Definition of Ready.

La persona responsable de preparar una Historia de Usuario debe asegurarse de que la información esté disponible antes del Refinement.

Durante el Refinement, el equipo debe identificar las dudas, dependencias y riesgos pendientes.

Durante el Sprint Planning, se debe confirmar nuevamente que las historias seleccionadas cumplen con la Definition of Ready.

Una Historia de Usuario que no cumpla los criterios necesarios no debe seleccionarse únicamente para completar la capacidad disponible del Sprint.

---

## 17. Documentos relacionados

* Definition of Done → `00-governance/definition-of-done.md`
* Agile Team Conventions → `00-governance/agile-conventions.md`
* Git Conventions → `00-governance/git-conventions.md`
* Documentation Rules → `00-governance/documentation-rules.md`
* Microservices Documentation → `00-governance/microservices-documentation.md`
* Security Policy → `00-governance/security-policy.md`
* Security Rules → `00-governance/security-rules.md`
* User Story Template → `04-requirements/_template-hu.md`
* User Stories Backlog → `04-requirements/user-stories.md`
* Functional Requirements → `04-requirements/functional.md`
* Non-functional Requirements → `04-requirements/non-functional.md`
* Business Rules → `04-requirements/business-rules.md`
* Architecture → `05-architecture/`
* Data → `06-data/`
