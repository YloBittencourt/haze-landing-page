# 🔍 Search Engine Optimization (SEO) & Tracking

## Estrutura Meta Tags (Head)
* **Title:** HAZE
* **Description:** HAZE. Ouça as faixas nas plataformas de streaming, acompanhe o trabalho e entre em contato. Página oficial do artista.
* **Theme Color:** `#0B0B0C` (Mimetiza a barra de status de navegadores mobile com o background do site).

## Open Graph (Social Sharing)
Configuração estratégica para gerar *Rich Cards* (Imagem, Título e Resumo) quando o link for compartilhado no WhatsApp, Instagram (DM) ou LinkedIn.
* **`og:url`:** `https://eohze.com`
* **`og:image`:** `/og-image.jpg` (Resolução: 1200x630px recomendada).
* **`og:type`:** `website`

## Semântica HTML5
* Uso rigoroso de `<header>`, `<nav>`, `<section>`, `<article>`, e `<footer>` para leitura clara por Screen Readers (Acessibilidade) e *Crawlers* do Google.
* Hierarquia de H-Tags respeitada (Um único `<h1>` no Hero, `<h2>` para títulos de seções, `<h3>` para títulos de álbuns/cards).

## Event Tracking (Google Analytics 4)
Os seguintes eventos foram mapeados via função JavaScript customizada `trackEvent(acao, local)` para mensuração de CRO:
1. `Clique_Spotify` (Origem: Header, Hero, Footer, Social Cards).
2. `Clique_YouTube` (Origem: Hero, Social Cards).
3. `Clique_WhatsApp` (Origem: Seção Contato, Footer).
4. `Clique_Email` (Origem: Seção Contato, Footer).