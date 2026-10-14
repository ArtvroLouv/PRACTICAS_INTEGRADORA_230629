# Práctica 06: Secuencia de pantallas — Spotify

## Descripción

Esta práctica presenta el flujo de experiencia de una aplicación móvil inspirada en Spotify. Incluye dos roles —oyente y artista—, las pantallas que comparten y las vistas específicas de cada recorrido.

## Entregables

- [Abrir los sketches interactivos](https://artvrolouv.github.io/PRACTICAS_INTEGRADORA_230629/Practica06/spotify-sketches.html): prototipos visuales de 18 pantallas con paleta oscura, verde y violeta, y una marca ilustrativa inspirada en Spotify.
- Diagrama Mermaid de secuencia que muestra la navegación entre pantallas y la bifurcación por rol.

El HTML es autocontenido: descarga o conserva el archivo junto a este README y ábrelo en un navegador para recorrer las secciones de pantallas compartidas, oyente y artista.

## Roles

- **Oyente:** explora recomendaciones, busca música, reproduce canciones, guarda playlists y consulta su biblioteca y perfil.
- **Artista:** entra a Spotify for Artists, revisa el panel, gestiona lanzamientos, consulta estadísticas y previsualiza su perfil público.

## Diagrama de secuencia

```mermaid
sequenceDiagram
    actor U as Usuario
    participant S01 as 1. Bienvenida
    participant S02 as 2. Elegir rol
    participant S03 as 3. Iniciar sesión
    participant S04 as 4. Crear cuenta
    participant S05 as 5. Permisos y preferencias
    participant S06 as 6. Inicio
    participant S07 as 7. Buscar
    participant S08 as 8. Resultados
    participant S09 as 9. Perfil
    participant S10 as 10. Biblioteca
    participant S11 as 11. Reproductor
    participant S12 as 12. Guardar en playlist
    participant S13 as 13. Spotify for Artists
    participant S14 as 14. Panel del artista
    participant S15 as 15. Música y lanzamientos
    participant S16 as 16. Estadísticas
    participant S17 as 17. Perfil público del artista
    participant S18 as 18. Configuración

    U->>S01: Abre la aplicación
    S01->>S02: Continuar
    U->>S02: Elige oyente o artista

    alt Usuario oyente
        S02->>S03: Acceder
        opt No tiene cuenta
            S03->>S04: Crear cuenta
            S04-->>S03: Cuenta creada
        end
        S03->>S05: Sesión iniciada
        S05->>S06: Elige preferencias y permisos
        U->>S06: Explora recomendaciones
        U->>S07: Toca Buscar
        S07->>S08: Escribe artista, canción o podcast
        S08->>S11: Selecciona un resultado
        U->>S11: Reproduce contenido
        S11->>S12: Guarda la canción
        S12->>S10: Elige o crea una playlist
        U->>S10: Abre su biblioteca
        S10->>S09: Consulta su perfil
        S09->>S18: Cambia ajustes de cuenta

    else Usuario artista
        S02->>S03: Acceder
        S03->>S05: Sesión iniciada
        S05->>S06: Elige preferencias y permisos
        S06->>S13: Abre Spotify for Artists
        S13->>S14: Accede al panel
        U->>S14: Revisa actividad
        S14->>S15: Gestiona música y lanzamientos
        S15->>S16: Consulta estadísticas
        S16->>S17: Revisa perfil público
        S17->>S18: Ajusta preferencias de cuenta
    end
```
