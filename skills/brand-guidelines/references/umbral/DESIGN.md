---
# gstack: design-md-format=spec
name: UMBRAL
typography:
  display:
    fontFamily: Unbounded
    fontWeight: 500
    letterSpacing: -0.02em
    lineHeight: 1.1
  body:
    fontFamily: Roboto
    fallback: Arial, sans-serif
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: Unbounded
    fontWeight: 400
    letterSpacing: 0.16em
    textTransform: uppercase
colors:
  petroleo: "#0F2C33"
  marfil: "#F3F0E8"
  laton: "#C4A062"
  laton-texto: "#7A5C25"
  salvia: "#A9BBAE"
  pizarra: "#4E6A70"
  texto-secundario: "#3E585E"
  primary: "{colors.laton}"
  background: "{colors.petroleo}"
  text: "{colors.marfil}"
spacing:
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  2xl: 96px
  3xl: 128px
rounded:
  none: 0px
  sm: 4px
  arch: 9999px 9999px 0 0
---

# Design System — UMBRAL

## Overview

- **Naming:** el umbral es la línea que se cruza al entrar a un hogar. Es una palabra real del español que se recuerda al instante y nombra el momento que la empresa acompaña.
- **Símbolo:** una n que se lee como un arco o una puerta abierta; el punto marca el paso del cliente.
- **Carácter:** emocional, sobrio y premium. Es la alternativa con más potencial narrativo.
- **Descriptor:** «Gestión Integral Inmobiliaria», en dos líneas, a la derecha del nombre.

## Colors

- **Enfoque:** sobrio y confiable. Remite a la arquitectura contemporánea y a los acabados nobles (puertas, manillas, placas). El latón es un detalle de terminación, no un color de relleno.
- **Proporción de uso:** petróleo + marfil ≈ 75 %, salvia y pizarra ≈ 17 %, latón ≈ 8 %.

| Token | Hex | Uso |
|---|---|---|
| petroleo | #0F2C33 | Fondo principal, logotipo positivo |
| marfil | #F3F0E8 | Fondo claro, texto sobre petróleo |
| laton | #C4A062 | Acento: arco, punto, foil, metal |
| laton-texto | #7A5C25 | Latón oscurecido, solo para texto sobre marfil |
| salvia | #A9BBAE | Superficies suaves, texto secundario sobre petróleo |
| pizarra | #4E6A70 | Textos de apoyo, líneas |
| texto-secundario | #3E585E | Párrafos sobre marfil |

**Pares de contraste aprobados**, medidos con la fórmula de WCAG 2.x:

| Texto | Fondo | Ratio | Uso permitido |
|---|---|---|---|
| petroleo | marfil | 12,9:1 | todo |
| salvia | petroleo | 7,3:1 | todo |
| petroleo | salvia | 7,3:1 | todo |
| texto-secundario | marfil | 6,7:1 | todo |
| laton | petroleo | 6,0:1 | todo |
| petroleo | laton | 6,0:1 | todo |
| laton-texto | marfil | 5,5:1 | todo |
| marfil | pizarra | 5,1:1 | todo |
| laton | marfil | 2,2:1 | **nunca para texto**; solo el punto o el arco del logotipo |

## Typography

- **Marca y titulares:** Unbounded, peso 500, tracking −0,02 em. Es ancha: calcula unos 0,75 em por carácter al dimensionar cajas.
- **Texto y descriptor:** Roboto 400/500, disponible en Google Fonts.
- **Etiquetas:** Unbounded 400 en mayúsculas, tracking 0,16 em, en latón sobre petróleo o en laton-texto sobre marfil.
- **Escala en presentación de 1920 × 1080:** 104 / 72 / 64 / 44 / 30 / 24 px. Nada bajo 24 px.
- **Escala web:** 64 / 44 / 32 / 24 / 18 / 16 px; párrafo de 16–18 px con interlineado 1,45.

## Layout

- **Área de resguardo:** la altura del arco (la n) alrededor de todo el logotipo.
- **Tamaños mínimos:**
  - Horizontal completo: 200 px / 50 mm. Es muy alargado: en formatos cuadrados usa el vertical.
  - Horizontal corto: 120 px / 30 mm.
  - Isotipo: 20 px / 7 mm.
- **Archivos de `assets/umbral/` según el fondo:**

| Fondo | Archivo |
|---|---|
| marfil o claro | `umbral-horizontal-positivo.svg`, `umbral-vertical-positivo.svg`, `umbral-horizontal-corto.svg` |
| petróleo u oscuro | `umbral-horizontal-negativo.svg`, `umbral-vertical-negativo.svg` |
| una tinta / grabado | `umbral-mono-negro.svg`, `umbral-mono-blanco.svg` |
| avatar, favicon, sello | `umbral-isotipo-laton.svg` (sobre petróleo), `umbral-isotipo-petroleo.svg` (sobre claro o latón) |
| solo nombre | `umbral-nombre.svg` |

- **Composición:** márgenes amplios (128 px en 1920) y titular arriba a la izquierda. El arco puede usarse grande y recortado como marco de fotografías.

## Elevation & Depth

- Diseño plano. Se admite un brillo radial muy suave en latón detrás del arco, solo en portadas y en video.
- El foil y el metal aparecen solo en piezas físicas y mockups.

## Shapes

- El arco es la forma madre: úsalo para marcos de imágenes, botones de cabecera redondeada (`rounded.arch`) y ventanas.
- El resto de las cajas son rectas, con radio de 4 px como máximo.
- El punto se puede usar como separador («·») entre servicios.

## Components

- **Jockey:** dos versiones.
  - Petróleo con el horizontal corto bordado: arco y punto en latón, nombre en marfil.
  - Marfil con el arco en bordado 3D petróleo y visera petróleo.
- **Polera:**
  - Frente petróleo con el arco en latón (serigrafía o foil).
  - Espalda marfil con el vertical de unos 25 cm: arco y punto en latón, nombre en petróleo, descriptor en pizarra.
- **Llavero de bienvenida:** cuero petróleo con el horizontal corto en hot stamping latón, argolla y llave doradas. Se entrega con una tarjeta marfil de 9 × 5,5 cm que dice «Bienvenido a tu nuevo hogar.» y lleva una franja latón en la base. Es la pieza que mejor cuenta el concepto: entregar las llaves es cruzar el umbral.
- **Presentaciones:** las portadas de sección van en petróleo, el contenido en marfil y la latón se reserva para etiquetas y detalles.

## Do's and Don'ts

- **Sí:** el latón en el arco y el punto; mucho aire; el arco como marco de fotografías.
- **Sí:** el nombre siempre en mayúsculas, tanto en el logotipo como en texto corrido.
- **No:** texto en latón sobre marfil (2,2:1).
- **No:** el horizontal completo en espacios cuadrados o pequeños.
- **No:** girar o invertir el arco; un arco al revés deja de ser una puerta.
- **No:** degradados dorados ni brillos metálicos en piezas digitales.
- **No:** combinar con FFF Acid Grotesk ni con Space Grotesk (son de GEINT).

## Motion

- **Clip de marca:** `assets/umbral/umbral-animacion.mp4`, 6 s, 1920 × 1080, fondo petróleo.
  1. 0,2 s: el arco se dibuja de izquierda a derecha, siguiendo su trazo como el de una puerta.
  2. 1,45 s: el punto aparece con un zoom (escala de 0 a 1 con un leve rebote).
  3. 2,05 s: una sola barra de luz latón recorre la línea y revela UMBRAL y el descriptor, ambos en marfil.
  4. 5,4 s: todo se desvanece.
- **Curva de animación:** cubic-bezier(.2, .8, .2, 1) para entradas y cubic-bezier(.6, 0, .2, 1) para la revelación del nombre.

## Decisions Log

| Fecha | Decisión | Razón |
|---|---|---|
| 2026-10-29 | Sistema inicial (propuesta) | Logotipo del cliente; paleta Petróleo y aplicaciones definidas en el brand kit de presentación. |
| 2026-10-29 | laton-texto #7A5C25 | El latón de marca da 2,2:1 sobre marfil; no sirve para texto. |
| 2026-10-29 | Vertical como versión para formatos cuadrados | El horizontal completo tiene proporción ~14:1 y se vuelve ilegible en espacios cuadrados. |
