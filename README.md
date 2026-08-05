# HAZE | Official Artist Landing Page 🎵

![Status](https://img.shields.io/badge/Status-Production_Ready-success?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

> **🔗 Live Preview:** [Acesse o site oficial aqui](https://haze-landing-page.vercel.app/)

Uma landing page premium, de alta performance e focada em conversão (CRO), desenvolvida para consolidar a presença digital do rapper HAZE. O projeto foi arquitetado para atuar como um *Hub Digital*, direcionando fãs para plataformas de streaming (Spotify/YouTube) e captando leads B2B (contratantes) de forma profissional.

---

## 🧠 UX/UI & Estratégia de Negócios

Como o foco do projeto é a indústria musical (Trap/Rap), a interface foi desenhada utilizando um padrão **Dark Mode** de alto contraste. Isso transmite sofisticação, destaca as *cover arts* dos lançamentos e reduz a fadiga visual, alinhando-se aos padrões de gigantes como Apple Music e Spotify.

*   **Arquitetura de Conversão (CRO):** CTAs estratégicos posicionados no Hero, Navbar e Footer, minimizando o atrito para o play na plataforma.
*   **Smart Tracklists:** Integração inteligente com iframes compactos do Spotify, criando uma experiência de "Leque" (Tracklist) nativa na própria página para Álbuns e EPs.
*   **B2B Booking:** Seção de contato blindada e otimizada para fechamento de shows, com redirecionamento via `mailto` e WhatsApp (`target="_blank"` para retenção de sessão).

---

## ⚡ Tecnologias & Arquitetura Técnica

Para garantir tempos de carregamento na casa dos milissegundos e uma pontuação máxima no Google Lighthouse, o projeto foi construído **sem dependências de frameworks pesados**, adotando a abordagem *Vanilla*.

*   **HTML5 Semântico:** Estruturação otimizada para leitores de tela e robôs de busca.
*   **CSS3 (Custom Properties):** Estilização moderna utilizando variáveis CSS para um sistema de design escalável, *Glassmorphism* no cabeçalho e responsividade nativa (Mobile-First).
*   **Vanilla JavaScript (ES6):** Utilizado para microinterações, controle do navbar no scroll e animações de *Scroll Reveal* usando a API `IntersectionObserver` (alta performance sem sobrecarregar a *main thread*).
*   **Google Analytics 4 (GA4):** Motor de inteligência de dados injetado de forma modular. Possui uma função global (`trackEvent`) disparando eventos customizados em todos os cliques críticos (Spotify, YouTube, WhatsApp, E-mail) para futura criação de públicos de Remarketing.
*   **SEO & Open Graph:** Meta tags configuradas para ranqueamento local ("Rapper em Ilhéus, Bahia") e geração automática de *Rich Cards* de alta resolução em compartilhamentos no WhatsApp/Instagram.


---

## 🚀 Como executar o projeto localmente

Como o projeto é estático e não requer *build steps*, a execução é imediata.

1. Clone o repositório:
   ``bash
   git clone https://github.com/SEU_USUARIO/haze-landing-page.git
   ``
2. Navegue até o diretório:
   ``bash
   cd haze-landing-page
   ``
3. Abra o arquivo `index.html` em seu navegador web ou utilize uma extensão como o *Live Server* no VS Code para injetar o protocolo `http://` e visualizar o rastreamento do GA4 no console.

---

## 👨‍💻 Desenvolvido por

**Ylo Silva de Sá Bittencourt**  
*Senior UI/UX Designer & Front-end Developer*