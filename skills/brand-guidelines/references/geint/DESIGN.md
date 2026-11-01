---
# gstack: design-md-format=spec
name: GEINT
typography:
  display:
    fontFamily: Unbounded
    fontWeight: 500
    letterSpacing: -0.02em
    lineHeight: 1.1
  body:
    fontFamily: FFF Acid Grotesk
    fallback: Space Grotesk, Arial, sans-serif
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: Unbounded
    fontWeight: 400
    letterSpacing: 0.16em
    textTransform: uppercase
colors:
  carbon: "#1F1E1C"
  hueso: "#F1ECE3"
  terracota: "#B9562F"
  terracota-texto: "#A24A27"
  arcilla: "#E2CBB2"
  hormigon: "#8A867D"
  texto-secundario: "#4A4741"
  primary: "{colors.terracota}"
  background: "{colors.hueso}"
  text: "{colors.carbon}"
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
  md: 8px
---

# Design System — GEINT

## Overview

- **Naming:** GEINT = **GE**stión + **INT**egral. Es un nombre corto y propio que funciona como firma, dominio y usuario de redes.
- **Símbolo:** una g minúscula coronada por un techo, calada en un cuadrado. Representa el hogar como centro de los cuatro servicios.
- **Carácter:** técnico, cercano y contemporáneo. Es la alternativa más versátil y clara.
- **Descriptor:** «Gestión Integral Inmobiliaria», en tres líneas, alineado a la izquierda junto al nombre.

## Colors

- **Enfoque:** cálido y material. Remite al ladrillo, la arcilla y el hormigón. Carbón y hueso dominan; la terracota se reserva para el acento.
- **Proporción de uso:** carbón + hueso ≈ 70 %, arcilla y hormigón ≈ 20 %, terracota ≈ 10 %.

| Token | Hex | Uso |
|---|---|---|
| carbon | #1F1E1C | Textos, fondos oscuros, logotipo positivo |
| hueso | #F1ECE3 | Fondo principal, texto sobre oscuro |
| terracota | #B9562F | Acento: isotipo, franjas, visera, cuero |
| terracota-texto | #A24A27 | Terracota oscurecida, solo para texto pequeño sobre hueso |
| arcilla | #E2CBB2 | Superficies secundarias, tarjetas |
| hormigon | #8A867D | Líneas, íconos, apoyos |
| texto-secundario | #4A4741 | Párrafos sobre hueso |

**Pares de contraste aprobados**, medidos con la fórmula de WCAG 2.x:

| Texto | Fondo | Ratio | Uso permitido |
|---|---|---|---|
| carbon | hueso | 14,2:1 | todo |
| texto-secundario | hueso | 7,9:1 | todo |
| carbon | arcilla | 10,6:1 | todo |
| terracota-texto | hueso | 5,0:1 | todo |
| #FFFBF5 | terracota | 4,6:1 | todo |
| carbon | hormigon | 4,6:1 | todo |
| terracota | hueso | 4,0:1 | solo ≥ 44 px o el logotipo |
| hueso | terracota | 4,0:1 | solo ≥ 44 px o el logotipo |
| terracota | carbon | 3,5:1 | solo ≥ 44 px o el logotipo |

## Typography

- **Marca y titulares:** Unbounded, peso 500, tracking −0,02 em. Es ancha: calcula unos 0,75 em por carácter al dimensionar cajas.
- **Texto y descriptor:** FFF Acid Grotesk (comercial, requiere licencia). Si no está disponible, usa Space Grotesk como sustituto y decláralo.
- **Etiquetas:** Unbounded 400 en mayúsculas, tracking 0,16 em, en terracota-texto o carbón.
- **Escala en presentación de 1920 × 1080:** 104 / 72 / 64 / 44 / 30 / 24 px. Nada bajo 24 px.
- **Escala web:** 64 / 44 / 32 / 24 / 18 / 16 px; párrafo de 16–18 px con interlineado 1,45.

## Layout

- **Área de resguardo:** ¼ del lado del isotipo alrededor de todo el logotipo.
- **Tamaños mínimos:**
  - Horizontal completo: 160 px / 40 mm.
  - Horizontal corto: 96 px / 25 mm.
  - Isotipo: 24 px / 8 mm. Para el favicon, usa el isotipo.
- **Archivos de `assets/geint/` según el fondo:**

| Fondo | Archivo |
|---|---|
| hueso o claro | `geint-horizontal-positivo.svg`, `geint-vertical-positivo.svg`, `geint-horizontal-corto.svg` |
| carbón u oscuro | `geint-horizontal-negativo.svg` |
| terracota | `geint-vertical-sobre-terracota.svg` |
| una tinta / grabado | `geint-mono-negro.svg`, `geint-mono-blanco.svg` (la g queda calada) |
| avatar, favicon, sello | `geint-isotipo-terracota.svg`, `geint-isotipo-carbon.svg` |
| solo nombre | `geint-nombre.svg` |

- **Composición:** márgenes amplios (128 px en 1920), titular arriba y a la izquierda, sin centrar el cuerpo.

## Elevation & Depth

- Diseño plano: sin sombras en la interfaz ni en los documentos.
- La profundidad (textura de tela, cuero o grano) aparece solo en mockups y fotografía de producto.

## Shapes

- El cuadrado del isotipo es la forma madre: usa cajas rectas con radio de 4 px como máximo.
- Recursos gráficos: franjas terracota de borde a borde y líneas de 2 px en carbón.

## Components

- **Jockey:** dos versiones.
  - Carbón con parche terracota bordado (isotipo).
  - Hueso con visera terracota y logotipo horizontal corto bordado.
- **Polera:**
  - Frente: isotipo de 8–9 cm a la altura del pecho, al lado izquierdo de quien la usa.
  - Espalda: vertical positivo de unos 25 cm.
  - Serigrafía al agua, sobre carbón u hueso.
- **Llavero de bienvenida:** cuero terracota con el horizontal corto en bajorrelieve y argolla plateada. Se entrega con una tarjeta hueso de 9 × 5,5 cm que dice «Bienvenido a tu nuevo hogar.» y lleva una franja terracota en la base.
- **Presentaciones:** fondo hueso; las portadas de sección van en carbón y las diapositivas de acento en terracota.

## Do's and Don'ts

- **Sí:** el isotipo solo en espacios pequeños; terracota como único acento; mucho aire alrededor del logotipo.
- **Sí:** el nombre en minúsculas («geint») dentro del logotipo; en texto corrido, «GEINT».
- **No:** cambiar la terracota por rojo o naranja saturado.
- **No:** poner el logotipo positivo sobre fotos sin una placa hueso detrás.
- **No:** separar el techo de la g ni usar la g sin su cuadrado.
- **No:** usar Unbounded en párrafos.
- **No:** combinar con Roboto (es la tipografía de UMBRAL).

## Motion

- **Clip de marca:** `assets/geint/geint-animacion.mp4`, 6 s, 1920 × 1080, fondo hueso.
  1. 0,2 s: el isotipo terracota entra con zoom y rebote sutil (escala 0,3 → 1,07 → 0,97 → 1,015 → 1, en 1,1 s).
  2. 1,05 s: el techo cae y se posa sobre la g con un pequeño rebote.
  3. 1,25 s: las letras de «geint» suben una a una, con 90 ms entre cada una.
  4. 2,05 s: entran las tres líneas del descriptor, sin línea separadora; a la vez (2,1 s) el techo hace su guiño: se eleva 4 px y vuelve a su lugar.
  5. 5,4 s: todo se desvanece.
- **Curva de animación:** cubic-bezier(.2, .8, .2, 1). Movimientos cortos y firmes, sin rebotes exagerados.

## Decisions Log

| Fecha | Decisión | Razón |
|---|---|---|
| 2026-10-29 | Sistema inicial (propuesta) | Logotipo del cliente; paleta Terracota y aplicaciones definidas en el brand kit de presentación. |
| 2026-10-29 | terracota-texto #A24A27 | La terracota de marca da 4,0:1 sobre hueso; texto pequeño necesita ≥ 4,5:1. |
| 2026-10-29 | Space Grotesk como sustituto | FFF Acid Grotesk es comercial; se usa el sustituto hasta tener licencia. |
