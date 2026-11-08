# 🔍 Search Engine Optimization (SEO) & Tracking

## Estrutura Meta Tags (Head)
* **Title:** HAZE | Novo Single CANGAÇO
* **Description:** HAZE. Novo single 'CANGAÇO' disponível no Spotify. Ouça as faixas nas plataformas de streaming, acompanhe o trabalho e entre em contato. Página oficial do artista.
* **Canonical URL:** `https://www.eohze.com/`
* **Theme Color:** `#0B0B0C` (Mimetiza a barra de status de navegadores mobile com o background do site).

## Rastreamento & Indexação (Crawlers)
* **`robots.txt`:** Permite livre indexação (`Allow: /`) e declara o caminho do sitemap.
* **`sitemap.xml`:** Lista a URL canônica `https://www.eohze.com/` com frequência de atualização semanal.
* **Schema.org (JSON-LD):** Metadados estruturados de `MusicGroup`, apontando Ilhéus (BA) como origem, links de redes sociais e canais de streaming.

## Open Graph & Twitter Cards (Social Sharing)
Configuração estratégica para gerar *Rich Cards* (Imagem, Título e Resumo) quando o link for compartilhado no WhatsApp, Instagram (DM), Facebook ou X/Twitter.
* **`og:url`:** `https://www.eohze.com/`
* **`og:image`:** `https://www.eohze.com/og-image.jpg` (Resolução: 1200x630px recomendada).
* **`og:type`:** `website`
* **`twitter:card`:** `summary_large_image`

## Semântica HTML5 & Performance de Mídia
* Uso rigoroso de `<header>`, `<nav>`, `<section>`, `<article>`, `<picture>` e `<footer>` para leitura clara por Screen Readers (Acessibilidade) e *Crawlers* do Google.
* Formato moderno **WebP** servido preferencialmente via `<picture><source type="image/webp">` com fallback transparente para navegadores legados via `<img>`.
* Atributos de dimensão intrínseca (`width` e `height`) e `loading="lazy"` para evitar Cumulative Layout Shift (CLS = 0).
* Hierarquia de H-Tags respeitada (Um único `<h1>` no Hero, `<h2>` para títulos de seções, `<h3>` para títulos de álbuns/cards).

## Event Tracking (Google Analytics 4)
Os seguintes eventos foram mapeados via função JavaScript customizada `trackEvent(acao, local)` para mensuração de CRO:
1. `Clique_Spotify` (Origem: Header, Hero, Footer, Social Cards).
2. `Clique_YouTube` (Origem: Hero, Social Cards).
3. `Clique_WhatsApp` (Origem: Seção Contato, Footer).
4. `Clique_Email` (Origem: Seção Contato, Footer).