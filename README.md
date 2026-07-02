# Gow Design System

Sistema de design mestre da Gow Agency e do João Musso. Fonte única de verdade visual, otimizado para uso com Claude (Claude Code, Claude Design e artifacts no claude.ai).

## Estrutura

- `DESIGN.md`: documento mestre e fonte da verdade (tokens `--gow-*`, princípios, tipografia, formatos)
- `foundations/cores.html`: paleta (10 tons, nunca #000/#FFF puros)
- `foundations/tipografia.html`: escala Neue Haas Grotesk e padrões de ênfase
- `foundations/logo.html`: monograma G, wordmark Grow/Own/Way, marca d'água
- `elements/componentes.html`: pill gow.agency (liquid glass), CTAs, hairlines, grid fantasma
- `backgrounds/fundos.html`: 4 famílias de fundo (seda escura, marca d'água, claro geométrico, foto P&B)
- `templates/feed-escuro.html`: capa de feed 1080×1350
- `templates/feed-claro.html`: capa de feed clara 1080×1350
- `templates/story.html`: story e reels 1080×1920
- `assets/`: logos oficiais (g-branco.svg, g-preto.svg, ícones PNG)

Cada HTML carrega o comentário `<!-- @dsCard group="..." -->` na primeira linha: é o formato que o Claude Design usa para indexar os cards. Os `<img src="../assets/...">` dependem da estrutura de pastas; não mover arquivos.

## Fonte

Neue Haas Grotesk Display, licenciada via Adobe Fonts. Não commitar arquivos de fonte. Sem a fonte instalada, os previews caem para Helvetica Neue.

## Nota técnica

Os `.svg` do logo são bitmaps mascarados, não vetor puro. O vetor original está em `02 Gow Agency/01 Identidade Visual/Gow/Cópia de G VETORIZADO.psd` caso precise exportar SVG de curvas.

## Nota

Este repositório substitui o `joaobrand` (arquivado). Uso interno: assets proprietários da Gow Agency e de João Musso.
