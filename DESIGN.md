# Gow Agency — Sistema de Design Mestre

> Grow Own Way. Minimalismo editorial, preto e prata, estética Apple.
> Fonte única: **Neue Haas Grotesk** (Display). Nunca cor pura, nunca ruído visual.

---

## 1. Princípios

1. **Menos, com intenção.** Um criativo = uma ideia. Espaço vazio é ativo, não sobra.
2. **Nunca a cor exata chata.** Preto sempre quente (`#0B0B0C`), branco sempre acinzentado (`#F4F4F2`). Zero `#000000` / `#FFFFFF`.
3. **Hierarquia por peso, não por cor.** A ênfase vem da variação Light → Regular → Bold da Neue Haas, do tamanho e da caixa-alta — não de cores de destaque.
4. **Geometria silenciosa.** Hairlines de 1px, o monograma G gigante em marca d'água (4–7% de opacidade), formas de canto arredondado. Presentes, nunca protagonistas.
5. **Liquid glass.** Superfícies translúcidas com blur e borda de 1px clara — a pill `gow.agency` é o exemplo canônico.
6. **Metáfora visual > ilustração literal.** Metrô que passa = quem espera não vende. iPhone = ferramenta sem estratégia. Objeto 3D flutuante sobre fundo claro = notícia/plataforma.
7. **Fotografia em P&B ou dessaturada**, contraste alto, sempre integrada ao fundo (nunca "colada").

---

## 2. Cor

| Token | Hex | Uso |
|---|---|---|
| `--gow-black` | `#0B0B0C` | Fundo escuro base |
| `--gow-ink` | `#141416` | Superfície escura elevada |
| `--gow-graphite` | `#1E1E20` | Cartões / blocos sobre escuro |
| `--gow-smoke` | `#2B2B2D` | Bordas e divisores sobre escuro |
| `--gow-steel` | `#6F6F6D` | Texto secundário sobre claro |
| `--gow-silver` | `#A6A6A4` | Texto secundário sobre escuro / títulos prata |
| `--gow-mist` | `#C9C9C7` | Detalhes, hairlines sobre claro |
| `--gow-fog` | `#DEDEDC` | Fundo claro alternativo |
| `--gow-paper` | `#E9E9E7` | Fundo claro base (off-white quente) |
| `--gow-white` | `#F4F4F2` | Texto sobre escuro |

Regras:
- **Duas famílias de fundo:** escuro (`black`→`graphite`, com gradiente sutil ou textura de seda) e claro (`paper`→`fog`, com geometria leve). Nunca meio-termo lamacento.
- Gradientes sempre tonais (preto→grafite, paper→fog), nunca coloridos.
- Vermelho, azul etc. só aparecem dentro de fotografia — nunca em UI/tipografia.

## 3. Tipografia

**Família:** `"Neue Haas Grotesk Display Pro", "neue-haas-grotesk-display", "Helvetica Now Display", "Helvetica Neue", Helvetica, Arial, sans-serif`

| Papel | Peso | Caixa | Specs (base 1080px) |
|---|---|---|---|
| Display hero | Bold (700) | ALTA | 96–150px · leading 0.98 · tracking -0.01em |
| Display misto | Light/Regular + palavras em Bold | ALTA ou Sentence | 72–110px · leading 1.02 |
| Título prata | Regular, cor `--gow-silver` | ALTA | usado em capas conceituais ("TRÁFEGO PAGO") |
| Subtítulo | Regular, itálico opcional | Sentence | 34–42px · leading 1.25 |
| Corpo | Regular | Sentence | 28–32px · leading 1.4 |
| Label / kicker | Regular + trecho Bold | ALTA | 20–24px · tracking 0.12em |
| Header "GOW AGENCY" | Regular | ALTA | 26px · tracking 0.18em |

Padrões de ênfase:
- **Palavra-chave em Bold dentro de frase Regular** ("nunca mais **perder clientes**").
- *Itálico* para conceito ("Anuncie com *estratégia*", "*As 6 etapas da confiança…*").
- Palavra com fundo invertido (barra `--gow-graphite` atrás de texto claro) para quebra de ritmo.
- Número gigante destacado (o "5") em Bold, cor `--gow-white`, sobreposto à foto.

## 4. Logotipo

- **Monograma G:** versão pequena no header (36–44px) e versão gigante em marca d'água (1.2–1.6× a largura do canvas, opacidade 4–7%, cortado pela borda).
- **Wordmark empilhado:** três linhas — **G**row / **O**wn / **W**ay — inicial em Bold, restante em Light. Usado como assinatura em peças de encerramento/outdoor.
- **"GOW AGENCY"** letterspaced no canto superior direito do header.
- Arquivos oficiais em `assets/`: `g-branco.svg` (fundo escuro), `g-preto.svg` (fundo claro), `icon-fundo-preto.png` / `icon-fundo-branco.png` (avatares e favicons). Nunca redesenhar ou distorcer o monograma.

## 5. Elementos recorrentes

- **Header padrão:** monograma G à esquerda + "GOW AGENCY" à direita + hairline de 1px abaixo (opacidade 30–40%). Margem superior ~64px.
- **Pill gow.agency (liquid glass):** raio total; fundo `rgba(255,255,255,.08)` (escuro) ou `rgba(0,0,0,.05)` (claro); borda 1px `rgba(255,255,255,.28)` / `rgba(0,0,0,.22)`; `backdrop-filter: blur(12px)`; texto 22px com "gow" Bold + ".agency" Regular.
- **CTA:** `ARRASTE PRO LADO ▶` ou `LEIA A LEGENDA ▼` — label caixa-alta, verbo Regular + objeto Bold, seta triangular pequena.
- **Hairline vertical** à esquerda de blocos de texto (1px, 40% opacidade, altura do bloco).
- **Grid fantasma:** linhas de 1px a 5–8% de opacidade cruzando o layout (estilo blueprint).
- **Grain:** ruído fino a 3–5% sobre fundos escuros (feTurbulence / textura), imperceptível mas orgânico.

## 6. Fundos

1. **Seda líquida escura** — ondas suaves preto/grafite com highlights prata (render ou foto de tecido), para peças de impacto.
2. **Marca d'água G** — fundo `--gow-black` ou `--gow-paper` com o monograma gigante recortado a 4–7%.
3. **Claro geométrico** — `--gow-paper` com formas de canto arredondado em `--gow-fog`/`--gow-mist` e grid fantasma.
4. **Fotografia integrada** — P&B/dessaturada, vinheta escura para ancorar o texto, sujeito sangrando na borda.

## 7. Formatos

| Formato | Canvas | Margens |
|---|---|---|
| Feed / carrossel | 1080×1350 | 84px laterais |
| Quadrado | 1080×1080 | 84px |
| Story / Reels | 1080×1920 | 96px laterais, zonas seguras 220px topo/rodapé |

---

*Fonte licenciada: Neue Haas Grotesk Display Pro (Adobe Fonts / Monotype). Nos previews HTML a pilha cai para Helvetica Neue quando a fonte não está instalada.*
