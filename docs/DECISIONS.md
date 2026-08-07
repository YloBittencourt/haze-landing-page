# ⚖️ Registro de Decisões Arquiteturais (ADR)

Este documento centraliza as principais decisões de engenharia, design e negócios tomadas durante o desenvolvimento, servindo como memória para futuras iterações. Toda atualização no projeto deve seguir o escopo documentado para preservar informações anteriores.

### 1. Stack Tecnológico (Vanilla vs. Frameworks)
* **Decisão:** Utilizar HTML5, CSS3 e JavaScript (ES6) puros (Vanilla).
* **Motivo:** Como trata-se de uma Landing Page estática com foco em máxima performance e SEO, o uso de frameworks como React/Next.js adicionaria um peso desnecessário (Bundle JS). O Vanilla garante carregamento em milissegundos, essencial para conexões móveis (3G/4G).

### 2. Infraestrutura e Separação de Responsabilidades (Agency Model)
* **Decisão:** Domínio na conta do cliente (Hostinger) e Código/Hospedagem na conta da agência/desenvolvedor (Vercel).
* **Motivo:** Protege a propriedade intelectual da marca do artista, enquanto mantém o controle técnico, de deploy e manutenção com o desenvolvedor, garantindo segurança operacional.

### 3. Renovação Automática do Domínio
* **Decisão:** Desativar a renovação financeira automática do `.com` na Hostinger.
* **Motivo:** Proteger os dados de faturamento do desenvolvedor e forçar um ponto de contato comercial anual com o cliente (Estratégia de Retenção).

### 4. Componentização Híbrida do Spotify
* **Decisão:** Usar embeds completos (152px) para Singles e embeds compactos agrupados (80px) para EPs (`.ep-tracklist`).
* **Motivo:** Evitar a poluição visual em projetos maiores (EPs), simulando a interface nativa de lista de reprodução do próprio aplicativo do Spotify.