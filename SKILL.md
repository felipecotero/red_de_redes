# Casa Común — Ministerio de las Culturas, las Artes y los Saberes

Skill for designing within the visual + content language of **Casa Común**, the institutional especial digital of the Colombian Ministerio de las Culturas, las Artes y los Saberes (2022–2026), and for products that live inside that universe — most notably an internal **Red de redes** (network-of-networks) of cultural and saberes organizations and territorial nodes.

## When to use

Use this skill when the user asks for designs, slides, prototypes, posters, web/app surfaces, or internal tools for:

- Casa Común itself, the repositorio, the agenda, or any sub-publication of it
- Mincultura institutional surfaces that should feel editorial / cultural rather than generic gov
- The **Red de redes** node-map and any directorio of organizations / territorios / pueblos / saberes
- Programming presented in the warm, communal, "casa de papel" register

## How to use

1. **Read `README.md`** for full content fundamentals, visual foundations, accessibility contract, and iconography rules.
2. **Import `colors_and_type.css`** at the top of every HTML file — it provides the full token set as CSS custom properties (`--cc-cream`, `--cc-coral`, `--cc-azul-noche`, `--cc-font-display`, `--cc-font-body`, `--cc-r-md`, etc.).
3. **Look at `preview/` cards** for canonical specimens of color, type, components, node-map nodes.
4. **Use `ui_kits/red_de_redes/index.html`** as the structural reference for the node-map / directorio surface — copy patterns from there rather than inventing.
5. Use **real photographs** for content imagery; never hand-roll SVG illustrations of people, pueblos, or wildlife. Cut-paper collage is the signature artwork — placeholder if not commissioned.
6. Voice: Spanish (Colombia), first-person plural, **tú** for invitations and **usted** for procedural copy, sentence case for heads, UPPERCASE only for small mono labels.

## Critical do's and don'ts

- ✅ **Do** use **Fraunces** (variable, opsz 144 on big heads, weights 400–600) for editorial display, **Nunito Sans** for body and UI — Nunito Sans is the institutional Mincultura spec.
- ✅ **Do** keep the **accessibility contract** visible on every public surface: skip link, A− / A / A+, *Alto contraste*.
- ✅ **Do** use the warm earth palette: cream paper, coral, terracotta, ochre, mostaza, verde musgo, azul noche.
- ✅ **Do** title sections in pairs — an evocative serif title above, a grounding subtitle below (*"Historias que sostienen la memoria" / "Territorios en resistencia"*).
- ✅ **Do** treat photographs as torn-paper-edge cards or behind a faint cream wash.
- ✅ **Do** use carousel chrome `‹` `›` `❚❚` and counters like *"Memoria 1 de 2"*.
- ❌ **Don't** invent SVG illustrations of people or pueblos — use real photos or commissioned cut-paper artwork.
- ❌ **Don't** use cool gradients, neon, or glassmorphism. Flat torn-paper edges where colors meet.
- ❌ **Don't** translate Indigenous-language phrases — preserve them verbatim.
- ❌ **Don't** use emoji in chrome.
- ❌ **Don't** uppercase headlines — sentence case. UPPERCASE is for eyebrows and a11y labels only.

## Red de redes specifics

When building the node-map UI kit:

- The graph is the centerpiece — nodes are circular, sized by tier (entidad adscrita > red regional > nodo local), colored from the secondary palette (ochre, verde musgo, azul cielo, mostaza, sand). The center node *Casa Común* / *Mincultura* is coral.
- Connections are thin `rgba(244,234,215,0.25)` lines on the azul-noche canvas, or `rgba(30,26,20,0.18)` on cream.
- A node detail panel slides in from the right with the organization's photo (torn edge), display-serif name, sentence-case description, and a tag rail of saberes / territorios / lenguas.
- A persistent filter rail uses the pill tag pattern from `preview/components-tags.html`.

## Notable files

- `colors_and_type.css` — design tokens
- `preview/` — color, type, spacing, component specimens (registered in the asset review pane)
- `ui_kits/red_de_redes/index.html` — node-map reference surface
