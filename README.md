# Modelos y Bases de Datos

JUAN SEBASTIÁN GUAYAZÁN CLAVIJO y MARIANELLA POLO PEÑA  
Modelos y Bases de Datos (ISIS MBDA-2 y MBDA-201)  
Decanatura Ingeniería de Sistemas → Centro de Estudios de Ingeniería de Software  
Ingeniería de Sistemas  
Escuela Colombiana de Ingeniería Julio Garavito  
2025-1

Repositorio general del curso: consolida los temas y conceptos vistos, y agrupa el proyecto, los laboratorios y los autoestudios como [submódulos de git](https://git-scm.com/book/en/v2/Git-Tools-Submodules) en las carpetas `Proyecto/`, `Laboratorios/` y `Autoestudios/` — cada uno con su propio detalle (enunciado, estructura, cómo ejecutar y resultados).

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

## Cómo clonar

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Modelos-y-Bases-de-Datos.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```

Para traer las últimas actualizaciones de cada repositorio enlazado:

```bash
git submodule update --remote --merge
```
