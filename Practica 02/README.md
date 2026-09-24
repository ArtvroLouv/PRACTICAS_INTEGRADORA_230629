
## Práctica 02 - Boceto de Arquitectura con Archify

### Evidencias de la práctica 02
Puedes consultar el documento completo de evidencias aquí: 
-> [Practica02_Boceto_Arquitectura_Archify.docx.pdf](/Evidencias/Practica02_Boceto_Arquitectura_Archify.docx.pdf) <-

[Ver arquitectura](https://artvrolouv.github.io/PRACTICAS_INTEGRADORA_230629/)

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