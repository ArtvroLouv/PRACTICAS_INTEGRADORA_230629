# Práctica 03: Implementación del Business Model Canvas de Spotify

[Ver Arquitectura](https://artvrolouv.github.io/PRACTICAS_INTEGRADORA_230629/Practica03/index.html)

## Descripción de la Práctica
En esta práctica se diseñó e implementó una interfaz web estructurada y responsiva que representa el Business Model Canvas (Lienzo de Modelo de Negocio) aplicado al servicio de streaming de audio Spotify.

El objetivo principal fue organizar de manera visual y accesible los nueve bloques estratégicos del modelo de negocio, complementándolos con una sección de hipótesis de validación y garantizando un diseño moderno y adaptable.

---

## Prompt Utilizado

```text
Actúa como un desarrollador Frontend experto en HTML5, CSS3 y JavaScript moderno.

Necesito que generes una aplicación web dinámica e interactiva que represente el Business Model Canvas (Lienzo de Modelo de Negocio) aplicado al servicio de streaming Spotify, basada en las siguientes especificaciones:

1. Estructura y Maquetación (HTML5 & CSS Grid):
   - Estructura semántica con etiquetas <header>, <main>, <section>, <article> y <footer>.
   - Distribución del lienzo usando CSS Grid de 5 columnas para reproducir la maquetación oficial del Business Model Canvas con los 9 bloques principales:
     * Socios clave (grid-row span 2)
     * Actividades clave
     * Recursos clave
     * Propuesta de valor (grid-row span 2)
     * Relación con clientes
     * Canales
     * Segmentos de clientes (grid-row span 2)
     * Estructura de costos (fila inferior)
     * Fuentes de ingreso (fila inferior)
   - Agrega un bloque o sección adicional al final para "Hipótesis de Validación".

2. Diseño Visual e Identidad (CSS3):
   - Usa variables CSS en :root con una paleta temática de Spotify (fondos oscuros, verde distintivo #1ED760, tonos menta, ámbar y violeta para destacar secciones específicas).
   - Estilo moderno utilizando cards independientes con gradientes suaves, bordes redondeados, sombras sutiles y tags/etiquetas de colores.
   - Totalmente responsivo utilizando @media queries (2 columnas en <= 900px y 1 sola columna en <= 540px).

3. Dinamismo y Funcionalidad (JavaScript Vanilla):
   - Haz que la información NO sea puramente estática. Define los datos de Spotify en una estructura/objeto JSON o arreglo dentro del código.
   - Renderiza dinámicamente las tarjetas (cards) y listas dentro de cada bloque del Canvas desde JavaScript.
   - Incluye interactividad dinámica:
     * Permitir agregar dinámicamente nuevas tarjetas/tarjetas de hipótesis desde un formulario modal o controles simples.
     * Filtros rápidos o búsqueda dinámica para resaltar tarjetas por categoría o tipo de cliente (ej. Usuarios Gratis vs. Suscriptores Premium).
     * Opción para colapsar/expandir o dar 'hover' interactivo a cada bloque para ver detalles del análisis.

Entrega el código limpio, bien comentado, utilizando buenas prácticas y listo para ejecutarse en un archivo único (o dividido en index.html, styles.css y script.js).
```

## Actividades Realizadas

1. **Estructuración Semántica del Documento (HTML5)**
   - Uso de etiquetas semánticas (`header`, `main`, `section`, `article`, `footer`) para asegurar accesibilidad y orden estructural.
   - Distribución de los 9 bloques del Canvas mediante elementos `article` identificados por id:
     - Socios clave
     - Actividades clave
     - Recursos clave
     - Propuesta de valor
     - Relación con clientes
     - Canales
     - Segmentos de clientes
     - Estructura de costos
     - Fuentes de ingreso
   - Adición de un bloque adicional para el análisis de hipótesis que requieren validación.

2. **Diseño Visual y Estilizado (CSS3)**
   - **Paleta de Colores y Tipografía:** Definición de variables CSS (`:root`) basadas en la identidad visual de la marca (tonos oscuros, verde distintivo `#1ed760`, tonos menta, ámbar y violeta para destacar secciones).
   - **Lienzo Principal con CSS Grid:** Configuración del contenedor `.canvas` mediante una cuadrícula de 5 columnas por 2 filas principales más una fila inferior, reproduciendo el maquetado oficial del Business Model Canvas.
   - **Posicionamiento Específico:** Uso de `grid-column` y `grid-row` para expandir bloques clave como *Socios clave*, *Propuesta de valor*, *Segmentos de clientes*, *Estructura de costos* y *Fuentes de ingreso*.
   - **Elementos de Interfaz:** Incorporación de etiquetas (`tags`), tarjetas independientes (`cards`) con degradados visuales y listas estilizadas para la presentación de los ingresos.

3. **Diseño Responsivo (Responsive Web Design)**
   - Implementación de reglas `@media` para garantizar una correcta lectura en dispositivos móviles y tabletas:
     - Dispositivos medianos (<= 900px): Reorganización de la cuadrícula a 2 columnas.
     - Dispositivos pequeños (<= 540px): Ajuste del flujo de lectura a 1 sola columna.

---

## Tecnologías Utilizadas

- **HTML5:** Lenguaje de marcado estructurado y semántico.
- **CSS3:** Hoja de estilos con variables CSS, gradientes, flexbox y cuadrículas responsivas (CSS Grid).