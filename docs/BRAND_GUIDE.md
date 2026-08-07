# 🎨 Brand Guide & Design System

## Tema Central
* **Vibe:** Urbano, Noturno, Psicodélico e Premium.
* **Paradigma:** Dark Mode Absolute.

## Paleta de Cores (CSS Variables)
* `--bg: #0B0B0C;` (Fundo primário, Preto puro/carvão).
* `--bg-panel: #151516;` (Fundo de cards primários).
* `--bg-panel-2: #1B1B1C;` (Fundo de cards secundários / *elevated*).
* `--line: rgba(245, 245, 243, 0.10);` (Divisórias e bordas sutis).
* `--ink: #F5F5F3;` (Branco *Off-White* para textos principais, evita cansaço visual).
* `--ink-dim: #B4B3B0;` (Cinza para parágrafos secundários).
* `--accent: #FFFFFF;` (Branco absoluto para botões primários e marcações).

## Tipografia (Google Fonts)
1. **Display & Headings:** `Bebas Neue`
   * *Uso:* Logo, H1, H2. Traz o impacto visual, letras condensadas, forte presença urbana.
2. **Body (Corpo do texto):** `Inter`
   * *Uso:* Parágrafos, botões e navegação. Legibilidade máxima em telas pequenas.
3. **Monospace (Detalhes técnicos):** `JetBrains Mono`
   * *Uso:* *Eyebrows* (tags de seção), metadados (datas, status). Traz um aspecto tecnológico e de "bastidores".

## Espaçamento & Grid
* Sistema de grid baseado em container de max-width `1140px`.
* Espaçamentos (Padding) fluidos via CSS `clamp()` para adaptação perfeita entre resoluções 4K, Desktop, Tablet e Mobile.