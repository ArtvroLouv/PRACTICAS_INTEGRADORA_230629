# Práctica 03: Implementación del Business Model Canvas de Spotify

## Descripción de la Práctica
En esta práctica se diseñó e implementó una interfaz web estructurada y responsiva que representa el Business Model Canvas (Lienzo de Modelo de Negocio) aplicado al servicio de streaming de audio Spotify.

El objetivo principal fue organizar de manera visual y accesible los nueve bloques estratégicos del modelo de negocio, complementándolos con una sección de hipótesis de validación y garantizando un diseño moderno y adaptable.

---

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