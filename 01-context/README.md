# 01 — Contexto del Proyecto

> **¿Qué es esto?** El "porqué" de Servi Te&Pro. Cualquier persona nueva en el proyecto debe poder leer esta carpeta y comprender qué problema resuelve el sistema, a quién está dirigido, qué incluye y qué se ha decidido deliberadamente dejar fuera.

## Por qué existe esta sección

Antes de diseñar e implementar el sistema, el equipo debe estar de acuerdo sobre:

* ¿Qué problema estamos resolviendo?
* ¿Para quién estamos resolviendo este problema?
* ¿Qué está dentro y qué está fuera del alcance?
* ¿Qué significa cada término empresarial y técnico?
* ¿Cuáles son los límites actuales del proyecto?

## Qué contiene esta sección y cómo completarla

### `overview.md` ⭐

Descripción ejecutiva del proyecto, con una extensión máxima de una página.

Debe incluir:

* Nombre del sistema.
* Problema que resuelve.
* Usuarios principales.
* Tecnologías principales.
* Estado actual del proyecto.

Formato sugerido:

```text
## ¿Qué es Servi Te&Pro?

[2-3 oraciones que describan el sistema...]

## Problema que resuelve

[Descripción del problema...]

## Usuarios principales

- Cliente...
- Técnico...
- Administrador...

## Stack tecnológico

- Frontend...
- Backend...
- Base de datos...
- Infraestructura...
```

### `scope.md` ⭐

Define los límites del proyecto:

* Qué está incluido en el alcance.
* Qué está fuera del alcance.
* Qué funcionalidades podrían incorporarse en versiones futuras.

### `glossary.md` ⭐

Diccionario de términos empresariales y técnicos utilizados en el proyecto.

### `_template-project-profile.md`

Plantilla para definir el perfil técnico y organizacional del proyecto.

### `_template-scope-declaration.md`

Plantilla para realizar una declaración formal del alcance del proyecto.

## Relación con otras secciones

* Problema definido en `overview.md` ↔ `03-product/vision.md`
* Alcance ↔ `04-requirements` y `03-product`
* Términos del glosario ↔ Todos los documentos
* Stack tecnológico ↔ `05-architecture`
* Límites del proyecto y supuestos principales ↔ `02-domain` y `05-architecture`

## Orden recomendado para completar esta sección

1. `overview.md`
2. `scope.md`
3. `glossary.md`

## Preguntas que esta sección debe responder

* ¿Qué es Servi Te&Pro?
* ¿Qué problema resuelve?
* ¿Quiénes son sus usuarios?
* ¿Cuál es el alcance del proyecto?
* ¿Qué funcionalidades están incluidas?
* ¿Qué funcionalidades están excluidas?
* ¿Qué términos debemos conocer para comprender el proyecto?
* ¿Cuáles son los límites y supuestos actuales?

## Estado actual

**En construcción**

Servi Te&Pro se encuentra actualmente en las fases de análisis, definición de requerimientos, diseño y construcción.
