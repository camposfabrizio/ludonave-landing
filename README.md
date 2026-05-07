# Ludonave Design System

## About the Brand

**Ludonave** is a modern board game rental service based in Navegantes (especially the Gravatá neighborhood), Santa Catarina, Brazil. They offer an acervo (collection) of modern board games for families, couples, friends, and hobbyists to rent for game nights at home or while visiting the region. They also operate **Ludonave Store** (game sales) alongside the rental service.

**Instagram:** [@ludonave.bg](https://instagram.com/ludonave.bg)  
**Target regions:** Navegantes, Gravatá, Penha, Balneário Piçarras, Itajaí, Barra Velha, Litoral SC

### Source Materials
- `uploads/MANUAL DA MARCA LUDONAVE.pdf` — Official brand manual (Canva, 9 pages, created 2026-04-29 by Fabrizio Silva Campos)
- `uploads/Duru_Sans,Exo,Squada_One.zip` — Font files (inaccessible due to filename; using Google Fonts equivalents — see caveat)

---

## CONTENT FUNDAMENTALS

### Tone of Voice
- **Convidativo (Inviting):** Welcomes all kinds of players, from first-timers to enthusiasts. Language feels warm and social.
- **Didático (Didactic):** Explains how the service works, what games are available, how to rent — educational without being dry.
- **Entusiasta (Enthusiastic):** Expressive, energetic; celebrates the joy of gaming. Uses exclamation marks naturally.

### Language
- **Portuguese (BR)** exclusively.
- Uses "você" (second person singular) addressing the reader directly — friendly and approachable.
- Casual but never sloppy. Short, punchy sentences mixed with warm invitations.
- No emoji overuse; occasional playful punctuation.
- Avoids corporate-speak. Reads like a game-night friend.

### Copy Examples
- "Acesse o acervo no link da bio e reserve seu jogo."
- "Chame no WhatsApp para garantir a diversão do finde."
- "Marque nos comentários quem vai jogar esse com você."
- "Qual seu tipo de jogo favorito? Responda abaixo."

### Hashtags
- **Nicho:** #ludonave #ludonavebg #jogosdetabuleiro #boardgamesbrasil #bggbrasil #jogosdemesa #gamenight
- **Geo:** #navegantes #gravata #penhasc #itajai #litoralsc #picarras #barravelha
- **Serviço:** #alugueldejogos #diversaoemcasa

### CTAs
- Rental: "Reserve seu jogo" / "Chame no WhatsApp"
- Engagement: "Marque quem vai jogar" / "Qual é o seu?"

---

## VISUAL FOUNDATIONS

### Color System
**Primary Palette:**
| Name | Hex | Usage |
|---|---|---|
| Vermelho Ludonave | `#bf0426` | Primary brand red; CTAs, hero accents |
| Amarelo Tabuleiro | `#f2bf27` | Secondary; highlights, badges, warmth |
| Azul Marinho | `#012030` | Deep navy; backgrounds, text on light |

**Secondary / Accent Palette:**
| Name | Hex | Usage |
|---|---|---|
| Branco | `#ffffff` | Text on dark, cards, surfaces |
| Verde Jogada | `#29a655` | Positive states, availability, go actions |
| Azul Claro | `#049dd9` | Info, links, interactive elements |
| Roxo Peão | `#6524bf` | Creative accent, special tags, variety |

### Typography
- **Display / Logo:** Squada One — bold, condensed, geometric. Used for brand name, large headlines, board-game aesthetic.
- **UI / Subheadings:** Exo — techy-geometric with humanist feel. Used for section titles, pricing, labels.
- **Body / Caption:** Duru Sans — friendly, readable sans-serif. Used for descriptions, body copy, UI text.

> ⚠️ Font files from the uploaded zip were inaccessible (special characters in filename). Google Fonts are used as drop-ins — visually identical.

### Backgrounds
- Deep navy (`#012030`) is the primary dark background.
- White and near-white are used for card surfaces.
- Vermelho and Amarelo used as bold accent/hero backgrounds for promo content.
- No heavy gradients; when used, they are subtle darkening overlays on photos.

### Imagery
- Photography: people playing board games, close-ups of game components, social gatherings.
- Warm, well-lit photography with a slightly saturated palette.
- Mockup-style flats for featuring specific games.
- No heavy filters; clean and inviting.

### Spacing & Layout
- Generous internal padding; content-forward design.
- Cards with subtle rounded corners (8–12px).
- Dense info sections use grid layouts; hero sections are spacious.

### Motion & Animation
- Subtle hover states: slight scale-up (1.03x), color shift.
- Transitions: 200ms ease-out.
- No complex animations; priority is clarity and speed.

### Borders & Shadows
- Cards: `box-shadow: 0 2px 12px rgba(1,32,48,0.12)` on white.
- Strong borders in brand colors used decoratively (e.g. left border accent for callouts).
- Border-radius: 8px for cards, 24px for pill buttons.

### Corner Radii
- Buttons: 24px (pill)
- Cards: 8–12px
- Badges/chips: 4–6px

### Iconography
See ICONOGRAPHY section below.

---

## ICONOGRAPHY

Ludonave does not use a custom icon font. The brand uses:
- **Phosphor Icons** (CDN: https://unpkg.com/phosphor-icons) — clean, friendly, rounded line icons. Best match for the brand's jovial-yet-clean aesthetic.
- Board-game themed icons: dice, chess pawns, users/groups, map pin, star.
- No emoji used as UI icons.

> The design system substitutes Phosphor Icons. If the brand manual specifies a different set, please supply it.

---

## FILE INDEX

```
README.md                          — This file (brand overview + guidelines)
SKILL.md                           — Agent skill definition
colors_and_type.css                — CSS variables: colors, typography, spacing
assets/
  logo_main.svg                    — Primary Ludonave logotype (SVG recreation)
  logo_icon.svg                    — Icon mark only (foguete)
  LOGO_COMPLETA.png                — Logotipo completo (PNG)
  mascote-vetor-preto.png          — Astronauta vetor com peão (fundo preto)
  mascote-vetor-rei.png            — Astronauta vetor de vitória (transparente)
  mascote-cabeca.png               — Sticker cabeça astronauta
  mascote-pixel.png                — Astronauta pixel-art com dados
  bg-galaxia.png                   — Fundo galáxia com balão (background placa)
  template-game-night.png          — Cena pixel completa GAME NIGHT
  template-game-night-v2.png       — Variante GAME NIGHT v2
  template-menu-pixel.png          — Folha de menu pixel original
  btn-jogador1.png                 — Botão pixel JOGADOR 1 (amarelo)
  btn-jogador2.png                 — Botão pixel JOGADOR 2 (vermelho)
  btn-opcoes.png                   — Botão pixel OPÇÕES (amarelo)
  btn-config.png                   — Botão pixel CONFIGURAÇÕES (vermelho)
  btn-escolher.png                 — Botão pixel ESCOLHER (pill amarelo)
fonts/                             — (Google Fonts used; no local files)
preview/
  colors-primary.html              — Primary color swatches
  colors-secondary.html            — Secondary/accent color swatches
  colors-semantic.html             — Semantic color usage
  type-display.html                — Display typography specimen
  type-body.html                   — Body/UI typography specimen
  type-scale.html                  — Full type scale
  spacing-tokens.html              — Spacing + radius tokens
  shadows-elevation.html           — Shadow + elevation system
  components-buttons.html          — Button variants
  components-badges.html           — Badges + chips
  components-cards.html            — Card patterns
  components-forms.html            — Input fields + form elements
  brand-logo.html                  — Logo usage
  brand-colors-combined.html       — Full color palette overview
  brand-mascote.html               — Astronauta Ludonave (4 versões) + foguete
  brand-stickers.html              — Stickers oficiais + composições prontas
  brand-elementos.html             — Lockups: ALUGUE E EXPLORE, GAME NIGHT, @ludonave.bg
  brand-padronagem.html            — Padrões com mascote + padrões geométricos
  brand-templates.html             — Botões pixel-art + templates GAME NIGHT + hero + notice
  type-special.html                — "Jogos de Tabuleiro" em 6 tratamentos + lockups
ui_kits/
  ludonave/
    README.md                      — UI kit notes
    index.html                     — Interactive prototype (main screen)
    Header.jsx                     — Navigation header
    GameCard.jsx                   — Game listing card
    HeroSection.jsx                — Hero / CTA area
    GameModal.jsx                  — Game detail modal
    Footer.jsx                     — Footer component
```
