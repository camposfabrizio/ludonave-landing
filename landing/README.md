# Landing Page — LUDONAVE

Landing page mobile-first em HTML estático puro, focada exclusivamente no **aluguel** de jogos de tabuleiro da Ludonave (Navegantes, Penha, Balneário Piçarras e Itajaí — SC).

## Estrutura

```
landing/
├── index.html      ← página completa (HTML + CSS inline)
└── README.md       ← este arquivo
```

A página consome recursos compartilhados da pasta-mãe `Rebranding/`:

- `../colors_and_type.css` — tokens de design, fontes, cores
- `../fonts/*.ttf` — Squada One, Exo, Duru Sans (carregadas pelo CSS)
- `../assets/*.png` — logo, mascotes, planetas, decorações pixel-art

## Como abrir

### Opção 1 — Direto no navegador (mais rápido)
Duplo-clique em `index.html`. Abre em `file://` e funciona na maioria dos navegadores modernos.

> Se as fontes locais não carregarem (alguns navegadores bloqueiam `@font-face` em `file://`), use a Opção 2.

### Opção 2 — Servidor local (recomendado)

```bash
# A partir da pasta Rebranding/
python -m http.server 8000
```

Depois acesse: <http://localhost:8000/landing/>

Alternativa Node:
```bash
npx serve .
```

## Seções

1. **Header fixo** — logo + navegação âncora + botão WhatsApp
2. **Hero** — headline "Embarque numa aventura de tabuleiro" + CTA `▶ ALUGUE AGORA`
3. **A Nossa Missão Espacial** — quem somos, regiões atendidas
4. **Manual de Voo (Como Alugar em 4 Passos)** — instruções diretas e literais
5. **Game Night** — CTA secundário com linguagem nerd/gamer descontraída
6. **Rodapé — A Base de Comando** — endereço, horários, redes sociais

## Links externos

| Onde | Destino |
|---|---|
| `▶ ALUGUE AGORA`, `🎲 ACESSAR O ACERVO`, `🎲 VER ACERVO COMPLETO` | <https://ludonave.acervodejogos.com.br/> |
| Botões WhatsApp (header e Game Night) | <https://api.whatsapp.com/send?phone=5547997082864> |
| `@ludonave.bg` (rodapé) | <https://instagram.com/ludonave.bg> |

Para trocar qualquer URL, basta buscar pela string no `index.html` e substituir — todas estão hardcoded.

## Stack

- HTML5 + CSS3 puros, single file
- Zero dependências de build (sem React, sem npm)
- Mobile-first com breakpoints em 600px, 768px e 1024px
- Fontes locais via `@font-face` + Press Start 2P do Google Fonts

## Acessibilidade

- `<html lang="pt-BR">`, `meta description`, `theme-color`
- Alt text em todas as imagens informativas; `aria-hidden` em decorativas
- `aria-label` em links de redes sociais
- Foco visível (outline amarelo) em todos os interativos
- `prefers-reduced-motion: reduce` desabilita animações
- Contraste validado: branco/navy (14.6:1), navy/amarelo (11.8:1)

## O que NÃO entra

Conforme briefing, a página **não menciona**:

- ❌ Venda de jogos / loja virtual
- ❌ Eventos com fornecimento de drinks
- ❌ Newsletter ou formulários de contato

CTAs sempre direcionam para o **acervo online** ou **WhatsApp**.

## Manutenção

Para alterar:

- **Texto** → editar diretamente o HTML (todas as strings inline)
- **Cores / espaçamentos / fontes** → editar `../colors_and_type.css` (afeta toda a marca)
- **Imagens decorativas** → trocar arquivos em `../assets/`
- **Layout / animações** → editar bloco `<style>` no topo do `index.html`
