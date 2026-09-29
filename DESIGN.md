---
name: Aurora — Portafolio Dark-Tech Premium
description: Glassmorphism con orbes de luz violeta-cian para el portafolio de Juan Calle Rosales.
colors:
  bg: "#070B16"
  bg-alt: "#0A101F"
  ink: "#EAF0FF"
  ink-dim: "rgba(234,240,255,0.66)"
  ink-faint: "rgba(234,240,255,0.54)"
  line: "rgba(255,255,255,0.10)"
  violet: "#8B7CFF"
  cyan: "#4FE0FF"
  pink: "#EC6BC8"
  grad: "linear-gradient(100deg,#8B7CFF,#4FE0FF)"
  on-accent: "#070B16"
  glass: "rgba(255,255,255,0.045)"
  bg-light: "#F3F6FC"
  bg-alt-light: "#EAEFF9"
  ink-light: "#0E1424"
  ink-dim-light: "rgba(14,20,36,0.70)"
  ink-faint-light: "rgba(14,20,36,0.64)"
  violet-light: "#6D5AE0"
  cyan-light: "#0891B2"
  grad-light: "linear-gradient(100deg,#6150D8,#0D6E88)"
  on-accent-light: "#FFFFFF"
typography:
  display:
    fontFamily: "Sora, system-ui, sans-serif"
    fontSize: "clamp(2.6rem,6vw,4.4rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.025em"
  section:
    fontFamily: "Sora, system-ui, sans-serif"
    fontSize: "clamp(1.8rem,3.6vw,2.6rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.85
    letterSpacing: "normal"
  label:
    fontFamily: "JetBrains Mono, ui-monospace, Menlo, Consolas, monospace"
    fontSize: "0.72-0.92rem"
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: "0.06-0.2em"
rounded:
  card: "18px"
  small: "10px"
  pill: "30px"
spacing:
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "34px"
  section: "100px 24px"
components:
  button-primary:
    backgroundColor: "{colors.grad}"
    textColor: "{colors.on-accent}"
    rounded: "12px"
    padding: "14px 28px"
  button-primary-hover:
    boxShadow: "0 12px 34px rgba(139,124,255,0.4)"
    transform: "translateY(-3px)"
  button-ghost:
    backgroundColor: "{colors.glass}"
    textColor: "{colors.ink}"
    border: "1px solid {colors.line}"
    rounded: "12px"
    padding: "14px 28px"
  chip:
    backgroundColor: "rgba(255,255,255,0.06)"
    textColor: "{colors.ink-dim}"
    border: "1px solid {colors.line}"
    rounded: "30px"
    padding: "6px 12px"
  glass-card:
    backgroundColor: "{colors.glass}"
    border: "1px solid {colors.line}"
    rounded: "18px"
    backdropFilter: "blur(14px)"
    boxShadow: "0 8px 32px rgba(0,0,0,0.22)"
---

# Design System: Aurora — Portafolio Dark-Tech Premium

## Overview

**Creative North Star: "El Producto de Cristal (The Glass Product)"**

El portafolio se presenta como un producto SaaS pulido, no como una tarjeta de presentación. El mundo es **dark-tech premium**: un fondo medianoche (`#070B16`) iluminado por orbes de luz desenfocados (violeta `#8B7CFF`, cian `#4FE0FF`, rosa `#EC6BC8`), con tarjetas de **vidrio esmerilado** (`backdrop-filter: blur`) que dejan respirar la luz de fondo. Los títulos importantes —incluido el nombre en el hero— usan el **gradiente violeta→cian** como acento de marca.

La personalidad es de software de alta gama: limpio, confiable, con elevación sutil al hover y una lectura cómoda en español. El visitante ve el trabajo como producto (Calletano POS, Calletano Web) y tiene un camino claro hacia proyectos y CV desde el primer viewport.

**Anti-referencia confirmada:** el mundo evita tanto el "terminal hacker" monocromo como el "cartel tipográfico"; el vidrio y el gradiente son la firma.

**Key Characteristics:**
- Orbes de luz desenfocados (violeta/cian/rosa) sobre medianoche.
- Tarjetas de cristal: relleno translúcido + blur + borde sutil.
- Acento gradiente violeta→cian en títulos, badges, números y enlaces fuertes.
- Esquinas suaves (18px en tarjetas, píldoras en chips), sin sombras duras.
- Sora (display) · Inter (body) · JetBrains Mono (labels/datos).
- Tema oscuro por defecto con claro opcional; `prefers-color-scheme` en primera visita.

## Colors

### Primary (Acento)
- **Violeta** (`#8B7CFF`) y **Cian** (`#4FE0FF`): los dos extremos del gradiente de marca. Se aplican juntos como `linear-gradient(100deg, #8B7CFF, #4FE0FF)` sobre texto (con `background-clip: text`) y sobre fondos de acción primaria.
- **Rosa** (`#EC6BC8`): solo como tercer orbe de fondo, muy atenuado.
- **En el tema claro los extremos de `--grad` divergen a propósito de los tokens decorativos.** `--grad` usa `#6150D8 → #0D6E88`, más oscuros que `--violet` (`#6D5AE0`) y `--cyan` (`#0891B2`). No es inconsistencia: `--violet` y `--cyan` viven en bordes, orbes y el punto de "disponible", donde nunca llevan texto encima; `--grad` sí es tinta y superficie de botón, y ahí los valores brillantes se quedaban en 3.19:1 y 4.35:1 (ver Contrast). Si mueves un extremo del gradiente, mueve también el otro y vuelve a medir.

### Neutral
- **Medianoche** (`#070B16`): fondo del sitio; `#0A101F` para secciones alternas.
- **Tinta** (`#EAF0FF`): texto principal.
- **Tinta atenuada** (`rgba(234,240,255,0.66)`): párrafos y descripciones. Medida: 7.22:1–7.71:1 en oscuro, 6.40:1–6.79:1 en claro.
- **Tinta tenue** (`rgba(234,240,255,0.54)`): tercera jerarquía — años de proyecto, copyright, label del hint de scroll. Medida: 5.26:1–5.44:1 en oscuro, 5.23:1–5.49:1 en claro.
- **Línea** (`rgba(255,255,255,0.10)`): bordes del vidrio.
- **Cristal** (`rgba(255,255,255,0.045)`): relleno de tarjetas glass; `rgba(255,255,255,0.07)` para estados reforzados.
- **Tinta sobre acento** (`--on-accent`: `#070B16` en oscuro, `#FFFFFF` en claro): el único color de texto admitido sobre una superficie pintada con `--grad`.

### Named Rules
**La Regla del Cristal.** Las superficies son vidrio: translúcidas, con blur y borde de 1px sutil, nunca rellenos opacos ni negros puros.

**La Regla del Gradiente.** El gradiente violeta→cian se reserva para acentos de marca (nombre en el hero, secciones destacadas, badges, números, botón primario, enlaces fuertes). Nunca se aplica como fondo de bloque grande.

**La Regla de un Solo Rol por Gradiente.** `--grad` cumple dos roles y cada uno impone una condición distinta: como **tinta** (con `background-clip: text`) necesita extremos suficientemente oscuros sobre fondos claros; como **superficie** necesita encima una tinta que contraste con ambos extremos. Un rol no se arregla moviendo el otro: si un CTA no contrasta, se cambia la tinta (`--on-accent`), no el gradiente.

**La Regla de la Tinta sobre Acento.** Sobre `--grad` solo se usa `--on-accent`. En oscuro es tinta oscura, porque el gradiente ya es brillante; en claro es blanca, porque el gradiente es profundo. Texto blanco sobre el gradiente oscuro daba 1.56:1.

## Contrast

**Objetivo:** WCAG 2.1 AA — 4.5:1 en texto normal y 3:1 en texto grande (≥ 24px, o ≥ 18.66px en negrita). Todo el texto se mide **compuesto sobre su fondo real**: las tintas son `rgba()`, así que su contraste depende del fondo que tengan debajo (medianoche, sección alterna o tarjeta glass con su propio blanco translúcido).

### Medición de referencia

| Token | Oscuro (peor caso) | Claro (peor caso) |
| --- | --- | --- |
| `--ink` | 15.19:1 | 15.92:1 |
| `--ink-dim` | 7.22:1 | 6.40:1 |
| `--ink-faint` | 5.26:1 | 5.23:1 |
| `--grad` como tinta (extremo violeta) | 5.30:1 | 4.99:1 |
| `--on-accent` sobre `--grad` | 6.01:1 | 5.76:1 |

Mínimo global del sitio: **5.30:1** en tema oscuro y **4.99:1** en claro, sobre 120 elementos de texto y 4 viewports por tema (1280 / 1024 / 768 / 390).

### Casos corregidos y su causa

| Síntoma | Valor que tenía | Causa | Corrección |
| --- | --- | --- | --- |
| CTA con texto blanco | 1.56:1 (oscuro) · 3.68:1 (claro) | blanco sobre el extremo cian del gradiente | tinta `--on-accent`: oscura en oscuro, blanca en claro |
| Labels, fechas, badges y enlaces en claro | 3.19:1–3.61:1 | `#0891B2` como tinta sobre fondos claros | extremos de `--grad` claro a `#6150D8 → #0D6E88` |
| Labels sobre sección alterna | 4.35:1 | `#6D5AE0` al límite sobre `--bg-alt` | igual que la fila anterior |
| Años, copyright y hint de scroll | 3.95:1 (oscuro) · 2.99:1 (claro) | `--ink-faint` demasiado tenue | alfa 0.44 → 0.54 (oscuro) y 0.46 → 0.64 (claro) |
| Skip link | 3.27:1 | blanco sobre `--violet` | fondo `--grad` + tinta `--on-accent` |

### Named Rules
**La Regla del Contraste Medido.** Ningún token de tinta se aprueba por su valor en el `:root`, sino por su peor caso compuesto. Tocar `--bg`, `--bg-alt`, `--glass` o cualquier extremo de `--grad` obliga a volver a medir las cuatro combinaciones de tema × fondo.

**La Regla del Techo del Tinte Tenue.** En el tema claro, `--ink-faint` no puede bajar de alfa ≈ 0.63: por debajo, sobre `--bg-alt`, sale de AA. Si hace falta una jerarquía más tenue, hay que bajar el fondo, no la tinta.

**La Regla del Texto Grande.** Los acentos de gradiente pueden quedarse brillantes solo en texto grande (nombre del hero, números de las métricas), donde el umbral es 3:1. En texto pequeño —labels de 0.72–0.8rem, badges, fechas, enlaces— el gradiente va oscuro.

## Typography

**Display Font:** Sora (fallback system-ui)
**Body Font:** Inter (fallback system-ui)
**Label/Mono Font:** JetBrains Mono (fallback ui-monospace, Menlo, Consolas)

**Character:** Sora da a los títulos un corte técnico pero amable (peso 800, tracking -0.025em); Inter mantiene el cuerpo legible en español; JetBrains Mono es la voz de los datos (labels de sección, chips, tags, años, stack). El mono se usa donde hay medición y estructura, nunca como disfraz del cuerpo.

### Hierarchy
- **Display** (Sora 800, `clamp(2.6rem, 6vw, 4.4rem)`, lh 1.1): nombre en el hero y titular del footer ("¿Trabajamos juntos?"). El apellido lleva el gradiente.
- **Section** (Sora 800, `clamp(1.8rem, 3.6vw, 2.6rem)`): títulos de sección.
- **Card Title** (Sora 700, `1.05–1.3rem`): títulos de tarjetas.
- **Body** (Inter 400, `1rem`, lh 1.85): párrafos, medida máx. ~60ch.
- **Label** (JetBrains Mono 500–600, `0.72–0.92rem`, tracking 0.06–0.2em, mayúsculas): labels de sección ("01 · Conóceme"), badges, tags, stack, años.

### Named Rules
**La Regla de la Voz Display.** Sora es la única voz display; sin serif ni otras sans display. JetBrains Mono para todo lo tabular con `font-variant-numeric: tabular-nums`.

## Layout

Una columna con hero centrado y secciones de ancho máx. 1080px (1160px en nav). El hero es centrado: avatar con anillo de gradiente, estado pill, nombre, rol, descripción (máx. 60ch), stack en mono y dos botones. Las secciones alternan fondo `bg`/`bg-alt`. Las habilidades usan grid de 3 columnas (2 a 1024px, 1 en móvil); proyectos en grid de 2; trayectoria en grid 1.5fr/1fr (timeline + side cards).

Responsive: a 1024px los grids bajan a 1 columna y la trayectoria apila; a 860px desaparecen los links de nav (hamburguesa); a 640px grids a 1 columna, contacto en columna y se oculta el hint de scroll.

## Elevation & Depth

La profundidad es **luz, no sombra dura**: los orbes de fondo aportan atmósfera; las tarjetas de cristal ganan elevación con hover (translateY(-4..-8px) + sombra violeta sutil `rgba(139,124,255,0.16-0.18)`). El navbar fijo añade blur y sombra al hacer scroll. Sin sombras duras negras ni glows excesivos.

### Named Rules
**La Regla del Hover Suave.** Elevar = elevar y teñir de violeta; nunca invertir el esquema ni romper el vidrio.

## Shapes

Esquinas suaves pero contenidas: **18px** en tarjetas grandes y glass, **10–12px** en botones y controles, **30px** (píldoras) en chips, badges y estado. Sin radios exagerados ni orgánicos. Los iconos de tecnologías (Devicon) entran en su color original; se evita monocromizarlos para no apagar el detalle.

### Named Rules
**La Regla del Radio Contenido.** Tres radios bastan (18 / 10–12 / píldora); ninguna forma libre.

## Components

### Tarjeta glass (`.glass`)
- **Forma:** relleno `rgba(255,255,255,0.045)` + `backdrop-filter: blur(14px)` + borde `rgba(255,255,255,0.10)` + radio 18px + sombra `0 8px 32px rgba(0,0,0,0.22)`.
- **Estado:** hover con `translateY(-4..-8px)` y sombra violeta; borde violeta en hover de proyectos.

### Botones
- **Primario (`.btn-primary`):** fondo gradiente violeta→cian, texto **`--on-accent`** (nunca blanco fijo: el gradiente oscuro no lo aguanta), radio 12px, mono mayúsculas; hover eleva con glow violeta.
- **Ghost (`.btn-ghost`):** glass + borde línea; hover tiñe el borde de violeta.
- **Focus:** `:focus-visible` con outline de 2px violeta.

### Chips
- **Estilo:** píldora, fondo `rgba(255,255,255,0.06)`, borde línea, mono 0.78rem, icono 18px; hover tiñe el borde de violeta y aclara el texto.

### Navbar (`.navbar`)
- **Estilo:** fijo, transparente hasta el scroll; al hacer scroll: glass con blur 18px y sombra sutil. Logo "JCR." con el punto en gradiente; CTA con gradiente y tinta `--on-accent`.

### Timeline (`.timeline`)
- **Estilo:** línea vertical, nodos circulares con borde violeta y glow `rgba(139,124,255,0.5)`; fechas en mono con gradiente.

### Proyectos (`.project-card`)
- **Tratamiento de capturas:** imagen con `saturate(0.95)`, zoom sutil al hover (scale 1.04).

## Do's and Don'ts

### Do:
- **Do** mantener la paleta medianoche + acento gradiente violeta→cian (La Regla del Gradiente).
- **Do** construir superficies como vidrio con blur y bordes sutiles (La Regla del Cristal).
- **Do** usar Sora para títulos y JetBrains Mono para labels y datos tabulares.
- **Do** elevar con hover suave y luz violeta (La Regla del Hover Suave).
- **Do** conservar SEO, Google Analytics, accesibilidad (skip-link, focus, reduced-motion) y el modo claro con `prefers-color-scheme`.
- **Do** usar `--on-accent` para cualquier texto sobre `--grad`, y `--ink-faint` para la tercera jerarquía de tinta (ya cumple AA en los dos temas).
- **Do** volver a medir el contraste tras tocar un fondo o un extremo del gradiente (La Regla del Contraste Medido).

### Don't:
- **Don't** usar negro puro como relleno de tarjetas ni sombras duras.
- **Don't** aplicar el gradiente a bloques grandes de fondo; es acento de marca.
- **Don't** introducir serif u otras display; Sora es la única voz display.
- **Don't** usar radios orgánicos ni formas libres.
- **Don't** separar secciones con iconos decorativos que no aporten significado; los labels mono con numeración cumplen esa función.
- **Don't** poner texto blanco sobre `--grad` en el tema oscuro (1.56:1), ni usar `--cyan` como color de texto pequeño sobre fondos claros (3.19:1).
- **Don't** bajar `--ink-faint` por debajo de alfa 0.54 (oscuro) / 0.64 (claro), ni usar `--violet` o `--cyan` como color de texto pequeño.
