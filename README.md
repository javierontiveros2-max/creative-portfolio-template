# Títutlo

## Subtítulo

> Encuentra aquí el proyecto deployado: [https://javierontiveros2-max.github.io/creative-portfolio-template/](https://javierontiveros2-max.github.io/creative-portfolio-template/)

## Descripción de los cambios realizados

Este README amplía la información del proyecto explicando qué se hizo en los archivos principales `index.html`, `404.html` y en los estilos ubicados en `assets/css/`. He conservado el contenido original arriba y añado a continuación las explicaciones detalladas.

**Resumen:**
- **Archivo principal:** `index.html` — estructura semántica, secciones de presentación y portafolio, y hooks para el JavaScript.
- **Página de error:** `404.html` — diseño coherente con el resto del sitio y un enlace para volver al inicio.
- **Estilos:** todos los archivos dentro de `assets/css/` organizan la apariencia, la accesibilidad, la responsividad y los componentes reutilizables.

**Nota sobre 4044.html:** en el repositorio se encuentra `404.html`; he documentado `404.html` asumiendo que te referías a esa página. Si existe un `4044.html` que quieres documentar específicamente, avísame y lo adapto.

---

## Detalle por archivo

**index.html**
- Estructura semántica: se utilizan etiquetas como `header`, `main`, `section` y `footer` para mejorar accesibilidad y SEO.
- Cabecera y navegación: incluye el menú principal con enlaces internos a secciones del portafolio.
- Sección principal (hero): contiene presentación, título y llamada a la acción para ver trabajos.
- Portafolio / proyectos: grid responsivo con tarjetas para cada proyecto. Las tarjetas están estilizadas con clases en los CSS y pueden enlazar a páginas o modales.
- Integración JS: el archivo `assets/js/main.js` (o `js/main.js`) enlaza interacciones como el menú responsive, animaciones suaves y mejoras de accesibilidad.

**404.html**
- Página de error personalizada: mantiene la identidad visual del sitio (tipografías, colores y estilos) y ofrece un enlace claro para volver al `index.html`.
- Diseño responsivo: ejecución de las mismas reglas CSS para que muestre bien en móvil y escritorio.

**assets/css/reset.css**
- Reinicia estilos por defecto de los navegadores para lograr una base consistente entre navegadores.

**assets/css/base.css**
- Define tipografías base, tamaño de texto, line-height, y variables CSS globales (colores, tamaños, etc.).

**assets/css/theme.css**
- Contiene las variables de color y esquemas temáticos (modo claro/oscuro si aplica). Aquí se centralizan los colores principales y secundarios.

**assets/css/layout.css**
- Define contenedores, grid y la estructura general de la página (anchos máximos, márgenes, sistemática de columnas y filas).

**assets/css/navigation.css**
- Estilos del menú principal, reglas para la versión desktop y mobile, incluyendo el comportamiento del icono 'hamburger' y las transiciones.

**assets/css/components.css**
- Estilos reutilizables para componentes: botones, tarjetas (cards), etiquetas (badges), formularios y otros elementos que se usan a lo largo del sitio.

**assets/css/index.css**
- Estilos específicos de la portada: ajustes para el hero, la disposición del portafolio en la página principal y pequeñas animaciones o efectos visuales aplicados sólo en `index.html`.
- Aquí fue donde intenté implementar la llamada "holographic card" (tarjeta holográfica) — ver nota de dificultades abajo.

**assets/css/responsive.css**
- Media queries y ajustes por puntos de quiebre para garantizar que la maquetación funcione correctamente en móviles, tablets y pantallas grandes.

**assets/css/accesibility.css**
- Reglas para mejorar la accesibilidad: enfoque visible en elementos interactivos (`:focus`), roles ARIA cuando aplica, tamaños mínimos de hit area y contrastes de color.

---

## Notas sobre la "holographic card"
- Intenté crear una tarjeta con efecto holográfico (degradados iridiscentes, brillo y sutiles animaciones 3D). Implementé la estructura HTML y varias reglas CSS (gradientes múltiples, mezcla de modos de fusión, filtros y transformaciones).
- Tuve dificultades para que el efecto fuese consistente entre navegadores y dispositivos; en particular, la combinación de `mix-blend-mode`, `backdrop-filter` y animaciones 3D no se comportó igual en todos los entornos. Por eso dejé una versión funcional pero simplificada para garantizar compatibilidad.
- Si quieres, puedo continuar iterando en la tarjeta holográfica usando soluciones progresivas (una versión CSS pura para navegadores modernos y una alternativa degradada para navegadores con menos soporte), o bien implementar la versión avanzada usando un pequeño canvas/WebGL si te interesa un resultado más fiel.
