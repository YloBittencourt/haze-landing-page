# 🧩 Arquitetura de Componentes UI/UX

O design foi concebido com uma estética de "Produto Digital Premium", mesclando referências de empresas do Vale do Silício com a identidade urbana do artista.

## 1. Ambient Background (Hero Section)
* **Estrutura:** `<div class="haze-field">` contendo `<div class="blob">`.
* **Comportamento:** Cria uma névoa psicodélica orgânica (*Haze*) usando gradientes radiais animados via CSS `@keyframes` (drift) rodando em loop infinito (20-28s) e sobreposto por um SVG Noise (Grain) overlay com `mix-blend-mode`.

## 2. Navigation Bar (Header)
* **Estrutura:** `<header id="site-header">`.
* **Comportamento:** Transparente no topo. Ao realizar o scroll (Intersection Observer), a classe `.scrolled` é injetada via JS, ativando um *Glassmorphism* pesado (`backdrop-filter: blur(14px) saturate(140%)`) e encolhendo o padding.

## 3. Cards de Discografia (`.release-card`)
* **Estrutura:** *CSS Grid* responsivo.
* **Comportamento:** Apresenta *hover state* duplo. O card sofre uma elevação suave eixo Y (`translateY`), enquanto a imagem interna (Cover Art) realiza um *Scale In* suave, gerando profundidade tátil sem quebrar o layout.

## 4. Botões e CTAs
* **`.btn-primary`:** Fundo branco sólido com texto preto, alto contraste, gerando foco imediato na ação principal (Ouvir no Spotify).
* **`.btn-ghost`:** Fundo transparente com borda fina (`rgba(255,255,255,0.1)`), utilizado para ações secundárias (YouTube/WhatsApp).

## 5. Scroll Reveal System
* **Comportamento:** Elementos com a classe `.reveal` iniciam invisíveis (`opacity: 0`) e deslocados. A API nativa do navegador `IntersectionObserver` detecta a entrada na viewport e injeta a classe `.in`, criando um efeito de cascata elegante sem dependência de bibliotecas externas pesadas.