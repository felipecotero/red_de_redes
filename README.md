# Casa Común — Design System
## Ministerio de las Culturas, las Artes y los Saberes · Colombia

> **Bienvenidos y bienvenidas a nuestra Casa Común**

A design system distilled from the **Casa Común** especial digital of the Ministerio de las Culturas, las Artes y los Saberes — a repositorio of contents 2022–2026 that frames Colombia as *"un país construido desde la diversidad de pueblos, lenguas, saberes y territorios."*

The institutional parent identity is **Colombia Potencia de la Vida · Gobierno del Cambio**, whose manual specifies **Nunito Sans** as the official institutional typeface. Casa Común layers on a more editorial / cultural register, using a serif display face (Fraunces in this kit, in the spirit of the original) for emotional, narrative weight.

This kit is built for an internal Mincultura product: **a node-map of the *Red de redes*** — the network of networks of cultural / saberes organizations and territorial nodes coordinated by the Ministry.

---

## Index

```
/
├── README.md                 (this file)
├── colors_and_type.css       — design tokens
├── SKILL.md                  — agent skill manifest
├── preview/                  — specimen cards
└── ui_kits/
    └── red_de_redes/         — node-map UI kit
        └── index.html
```

---

## CONTENT FUNDAMENTALS

**Language.** Spanish (Colombia). Inclusive doubles where appropriate (*"bienvenidos y bienvenidas"*). Indigenous-language phrases are preserved verbatim and never translated.

**Voice.** Institutional but warm and convivial — *"nuestra Casa Común"*, never *"el repositorio del Ministerio."* First-person plural ("nosotros / nosotras") signals collective ownership across pueblos and territorios.

**Tú vs. Usted.** Mixed by surface: **tú** in invitations and exploration ("Recorre nuestra Casa Común", "Descubre aquí"); **usted** in formal procedural contexts ("Consulte la agenda", "Use los filtros").

**Casing.**
- **Title Case** for section heads (*"Historias que sostienen la memoria"*, *"Somos mirada"*, *"Voces que cuidan el territorio"*).
- **Sentence case** for body and descriptive paragraphs.
- **UPPERCASE only for** small mono labels (eyebrows, accessibility toggles, footer credits).

**Tone.** Editorial, ceremonial, territorial. Recurring lexicon:
- *territorio · saberes · memoria · voces · lenguas · ritmos · acentos · acompañar · convivir · tejido · diversidad · pluralidad · pueblos · raíz · escuchar · cuidar · habitar*

**Section signatures (always in pairs):** an evocative title above, a subtitle that grounds it.
- *"Historias que sostienen la memoria"* → "Territorios en resistencia"
- *"Voces que cuidan el territorio"* → "Relatos colectivos y saberes en movimiento"
- *"Somos mirada"* → "Galerías, piezas y relatos visuales para recorrer el territorio desde otras perspectivas"
- *"Somos sonido, somos voces"* → "Lenguas, memorias, acentos y ritmos que habitan nuestra Casa Común"

**Numbers.** Stated plainly: *"270 actividades · 88 editoriales · 15 territorios"*.

**Calls-to-action.** Short verbal invitations, sentence case: *"Explorar contenidos"* · *"Ver destacados"* · *"Leer más"* · *"Descubre aquí"* · *"Escucha aquí"* · *"Seleccionar temática"*.

**Emoji.** Not used in chrome.

---

## VISUAL FOUNDATIONS

### Mood
**Casa de papel** — the central metaphor is a *house* built collaboratively from layered cut-paper figures, foliage, performers, and territorial silhouettes. Warm, daylight, communal. It feels like a beautifully art-directed museum especial — a collage on cream paper with a soft serif voice.

### Color
A warm earth palette, no cool gradients.
- **Cream `#f4ead7`** — page base, paper.
- **Coral `#d8634b`** — primary accent, the warm coral of the cut-paper performers.
- **Terracotta `#a4422c`** — deep accent for figures and CTAs.
- **Ochre `#c8924a`** + **mostaza `#d4a836`** — labels, highlights, sun.
- **Verde musgo `#4f6b3a`** — foliage in the collage.
- **Azul noche `#2a3552`** — deep type on cream, navigation, "night sky" sections.
- **Tinta `#1e1a14`** — body text, near-black.

There is **no purple, no neon, no cool gradient slop**. Where colors meet, they're flat or come together as torn-paper edges.

### Type
- **Body: Nunito Sans** (300/400/600/700/800/900) — institutional spec from Mincultura's manual.
- **Display: Fraunces** (variable, opsz 9–144) — a soft editorial serif that handles the warm, ceremonial register of Casa Común. Use weights 400–600; let opsz=144 expand on big heads.
- **Display tracking** is slightly tight (`-0.015em`); body normal.
- **Italics** carry feeling — used in pull-quotes and editorial captions.
- **Sentence case for heads** (not uppercase). UPPERCASE is reserved for small mono labels with `letter-spacing: 0.18em`.
- The accessibility nav (A− · A · A+ · Alto contraste) is a fixed contract — keep its visual treatment whenever you build a public surface.

### Backgrounds & imagery
- **Layered cut-paper collage.** The signature device is a hero with PNG-with-transparency *layer* PNGs (`layer-performer.png`, `layer-right-figure.png`) of performers / dancers / botanic motifs stacked over a cream background.
- **Photographs** of programming / cultural events appear as **torn-paper-edge cards** or behind a faint cream wash.
- **Botanical and territorial silhouettes** (palm fronds, mountains, river curves) anchor compositions at the edges.
- **Wave / agua undulada motif** is inherited from the parent identity (Colombia Potencia de la Vida) — used sparingly as a decorative line element.
- **No SVG illustrations of people.** Use real photos or commissioned cut-paper artwork.

### Animation
- **Soft fades over hard cuts.** Carousel transitions ~0.6s ease.
- **Layered parallax** on hero collage (rear figures translate slower than front).
- **Hover lifts** on cards: `translateY(-2px)` + warmer shadow.
- **Carousel arrows** ‹ / › with pause `❚❚` icon — keep the dingbat treatment from the source.

### Borders & cards
- Card surface: `#ffffff` or `#f7eed9` on cream. **No translucent glass.**
- Border: `1px solid rgba(30,26,20,0.12)` — barely there.
- Radius: cards 14–22px, big feature blocks 36px, pills 9999px.

### Shadow systems
- **Warm, soft, papery** — `0 6px 18px rgba(80,50,20,0.10)`. No cold blue shadows.
- Hover bumps to `0 16px 40px rgba(80,50,20,0.16)`.

### Layout rules
- **Generous side margins** on the cream background — never edge-to-edge text.
- **Editorial column widths** for body copy (max ~640px).
- **Asymmetric collage compositions** for hero and storytelling sections — figures push off-center.
- **Carousel with counter** ("Memoria 1 de 2") at the bottom of looping content.
- **Section bands** alternate cream → cream-deep → azul-noche; never coral as a full background, always as accent.

### Iconography
- **Material Symbols Outlined** for system glyphs (search, filter, close, play, arrow). Outlined weight 400, optical size 24, fill 0.
- **Unicode dingbats** allowed for carousel chrome: `‹` `›` `❚❚` `×`.
- **Real photographs** for content imagery.
- **No hand-rolled SVG illustrations.** If a glyph is missing, use Material Symbols.

---

## ACCESSIBILITY (a contract, not a feature)

Casa Común exposes accessibility controls at the very top of the page:
- **Skip link** — "Saltar al contenido" → `#contenido-principal`
- **Font size: A− · A · A+**
- **Alto contraste** toggle

Any product built in this system MUST keep these controls visible (either in the nav or a fixed corner button). Treatment can be small uppercase mono buttons in azul noche — see `colors_and_type.css :: .cc-a11y-nav`.

---

## CAVEATS

- The original Casa Común uses custom `layer-performer.png` and `layer-right-figure.png` cut-paper compositions. They are not bundled here (asset rights). Use placeholders or commission new collages.
- `Fraunces` is used as a stand-in for the editorial serif feel — if Mincultura has commissioned a different display serif for Casa Común specifically, swap in `--cc-font-display`.
- **Nunito Sans is canonical** for body / UI per the institutional manual.
