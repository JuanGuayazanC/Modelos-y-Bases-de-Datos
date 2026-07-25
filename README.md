# Modelos y Bases de Datos

JUAN SEBASTIÁN GUAYAZÁN CLAVIJO y MARIANELLA POLO PEÑA  
Modelos y Bases de Datos (ISIS MBDA-2 y MBDA-201)  
Decanatura Ingeniería de Sistemas → Centro de Estudios de Ingeniería de Software  
Ingeniería de Sistemas  
Escuela Colombiana de Ingeniería Julio Garavito  
2025-1

Índice del proyecto, los laboratorios y los autoestudios del curso, separados cada uno en su propio repositorio y enlazados aquí como [submódulos de git](https://git-scm.com/book/en/v2/Git-Tools-Submodules) — cada carpeta es un puntero al repositorio real, no una copia de su contenido.

## Temas del curso

El curso recorre el ciclo completo de diseño e implementación de una base de datos relacional, con extensión a XML:

| Tema | Dónde se trabaja |
|---|---|
| Introducción al modelo relacional | — |
| Diseño conceptual (general y extendido) | Laboratorios 01–02, Autoestudios 01–02 |
| Modelo relacional y SQL Developer | Autoestudio 03 |
| Integridad declarativa | Laboratorio 03, Autoestudio 04 |
| Integridad procedimental (PL/SQL) | Laboratorio 04, Autoestudio 04 |
| Diseño físico, componentes y paquetes | Laboratorio 05, Autoestudio 05 |
| Transacciones | Autoestudio 05 |
| Seguridad | Laboratorio 05, Autoestudio 05 |
| XML y su integración a SQL | Laboratorio 06, Autoestudio 06 |
| Normalización | — |

## Motores y herramientas

- **Oracle** (SQL Developer) — motor principal desde el Autoestudio 03 en adelante: DDL/DML, restricciones declarativas y procedimentales (triggers, paquetes), transacciones, seguridad por roles, y extensiones XML (`XMLType`).
- **MySQL** (vía [SQLZoo.net](https://sqlzoo.net/)) — usado en los primeros laboratorios y autoestudios para consultas SQL básicas y de junta, sobre los casos Adventure Works y University Timetables.
- **[Astah](https://astah.net/)** — modelado UML: diagramas de clases (modelo conceptual y lógico) y de casos de uso (funciones, consultas operativas).

## Proyecto

**ECINotes** — sistema de gestión académica para estudiantes de la Escuela Colombiana de Ingeniería: registro de materias, cálculo de promedios y visualización del progreso en el plan de estudios, con base de datos relacional en Oracle.

| Carpeta | Repositorio |
|---|---|
| `Proyecto` | [SICEI-MBDA](https://github.com/JuanGuayazanC/SICEI-MBDA) |

## Laboratorios

| Carpeta | Repositorio |
|---|---|
| `Laboratorios/Diseno-Conceptual-General-MBDA` | [Laboratorio 01: Diseño Conceptual General. SQL-DQL Básico](https://github.com/JuanGuayazanC/Diseno-Conceptual-General-MBDA) |
| `Laboratorios/Diseno-Conceptual-Extendido-MBDA` | [Laboratorio 02: Diseño Conceptual Extendido. SQL - DQL](https://github.com/JuanGuayazanC/Diseno-Conceptual-Extendido-MBDA) |
| `Laboratorios/Diseno-Logico-Declarativo-MBDA` | [Laboratorio 03: Diseño Lógico. Declarativo. SQL - DDL, DML](https://github.com/JuanGuayazanC/Diseno-Logico-Declarativo-MBDA) |
| `Laboratorios/Diseno-Logico-Procedimental-MBDA` | [Laboratorio 04: Diseño Lógico. Procedimiental. SQL - DDL, DML](https://github.com/JuanGuayazanC/Diseno-Logico-Procedimental-MBDA) |
| `Laboratorios/Diseno-Fisico-MBDA` | [Laboratorio 05: Diseño Físico. SQL-DTL-TCL](https://github.com/JuanGuayazanC/Diseno-Fisico-MBDA) |
| `Laboratorios/XML-y-SQL-MBDA` | [Laboratorio 06: XML y SQL](https://github.com/JuanGuayazanC/XML-y-SQL-MBDA) |

## Autoestudios

| Carpeta | Repositorio |
|---|---|
| `Autoestudios/SQL-Basico-Consultas-MBDA` | [Autoestudio 01: SQL Básico — Consultas](https://github.com/JuanGuayazanC/SQL-Basico-Consultas-MBDA) |
| `Autoestudios/SQL-Basico-Juntas-MBDA` | [Autoestudio 02: SQL Básico — Juntas y conjuntos](https://github.com/JuanGuayazanC/SQL-Basico-Juntas-MBDA) |
| `Autoestudios/SQL-Developer-MBDA` | [Autoestudio 03: SQL Developer](https://github.com/JuanGuayazanC/SQL-Developer-MBDA) |
| `Autoestudios/PLSQL-Basico-Declarativo-MBDA` | [Autoestudio 04: PL/SQL Básico — Restricciones declarativas](https://github.com/JuanGuayazanC/PLSQL-Basico-Declarativo-MBDA) |
| `Autoestudios/PLSQL-Basico-Paquetes-MBDA` | [Autoestudio 05: PL/SQL Básico — Paquetes](https://github.com/JuanGuayazanC/PLSQL-Basico-Paquetes-MBDA) |
| `Autoestudios/XML-Basico-MBDA` | [Autoestudio 06: XML Básico](https://github.com/JuanGuayazanC/XML-Basico-MBDA) |

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
