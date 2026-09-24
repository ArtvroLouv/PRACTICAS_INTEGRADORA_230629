# Prácticas Integradora

Repositorio correspondiente a las prácticas de la materia Integradora, donde se almacenan las actividades, evidencias, documentos y proyectos realizados durante el curso.

## Información

| Dato | Información |
|---|---|
| **Alumno** | José Arturo García González |
| **Materia** | Integradora |
| **Grupo** | 10.º |
| **Repositorio** | `PRACTICAS_INTEGRADORA_230629` |
| **Año** | 2026 |

---

## Tabla de prácticas

| No. | Práctica | Descripción | Estado |
|---:|---|---|:---:|
| 01 | Práctica 01 | Actividades correspondientes a la primera práctica de la materia | Concluida |
| 02 | Pràctica 02 | Boceto de arquitectura con Archify y Codex <br> [Ver arquitectura](https://artvrolouv.github.io/PRACTICAS_INTEGRADORA_230629/) | Concluida |

---

## Práctica 02 - Boceto de Arquitectura con Archify

En esta práctica se realizó la instalación y configuración del agente de modelado arquitectónico **Archify**, utilizando **Codex** para generar un primer boceto interactivo de la arquitectura del proyecto integrador.

La arquitectura propuesta contempla los siguientes componentes:

- Flutter Mobile App
- Keycloak Authentication
- FastAPI REST API
- PostgreSQL
- MongoDB
- Leaflet / Maps Service
- Docker
- Docker Compose
- Git
- GitHub

### Arquitectura del sistema

```text
Flutter Mobile App
        |
        +----> Keycloak Authentication
        |
        +----> FastAPI REST API
                    |
                    +----> PostgreSQL
                    |
                    +----> MongoDB
        |
        +----> Leaflet / Maps Service

Development Environment
        |
        +----> Docker
        |
        +----> Docker Compose

Source Control
        |
        +----> Git
        |
        +----> GitHub