# Modelos y Bases de Datos (MBDA)

Repositorio general del curso. Para saber cómo aprovecharlo, ver [Cómo usar este repositorio](#cómo-usar-este-repositorio).

## Estructura del proyecto

```
Modelos-y-Bases-de-Datos/
├── Proyecto/        # Submódulo → SICEI-MBDA
├── Laboratorios/     # Submódulos → un repo por laboratorio
└── Autoestudios/      # Submódulos → un repo por autoestudio
```

## Temas del curso

El curso recorre el ciclo completo de diseño e implementación de una base de datos relacional, con extensión a XML:

- Introducción al modelo relacional.
- Diseño conceptual, general y extendido (grandes conceptos, funciones, consultas operativas).
- Diseño lógico, con mecanismos de integridad declarativa (restricciones, claves) y procedimental (triggers, acciones referenciales).
- Diseño físico: componentes empaquetados, transacciones, seguridad por roles.
- Normalización.
- XML: consultas XPath, esquemas DTD, e integración de datos semiestructurados a un modelo relacional.

## Cosas a tener en cuenta

- El curso trabaja en dos motores según la etapa: **MySQL** (vía SQLZoo.net) al inicio, para consultas SQL básicas y de junta; y **Oracle** (SQL Developer) desde el diseño lógico en adelante, para DDL/DML, PL/SQL, transacciones y seguridad.
- El modelado (conceptual, lógico y de casos de uso) se hace en **Astah**, y se espera que el modelo quede trazable al código: cada regla de integridad implementada debe estar también documentada en el diseño.
- La convención de nombres de restricciones (`PK_`, `UK_`, `FK_`, `CK_`) y de comentarios por sección (`CICLO N: <sección>`) se mantiene a lo largo de todo el curso, del primer laboratorio al último.
- El desarrollo se organiza por ciclos: se implementa primero un subconjunto acotado del dominio (un CRUD o área funcional), y se extiende gradualmente, en vez de construir todo el modelo de una vez.

## Herramientas

- **[SQLZoo.net](https://sqlzoo.net/)** — motor MySQL, consultas SQL básicas.
- **Oracle / SQL Developer** — motor principal desde el diseño lógico en adelante.
- **[Astah](https://astah.net/)** — modelado UML (clases y casos de uso).

## Profesores

Laura Catalina Herrera Correa (teoría) y María Irma Díaz Rozo (laboratorio).

## Cómo usar este repositorio

Este repositorio no contiene código directamente: es una colección de repositorios independientes (proyecto, laboratorios y autoestudios), organizados por carpetas. Cada carpeta es un submódulo de git que apunta al repositorio real de esa actividad.

- **Para consultar una actividad puntual**: entra directamente a su carpeta en GitHub (o navega el submódulo) y revisa su propio README.
- **Para tener todo el contenido en tu máquina**:

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Modelos-y-Bases-de-Datos.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```
