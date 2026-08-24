<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&pause=1000&color=2E9EF7&center=true&vCenter=true&width=650&lines=Ol%C3%A1%2C+eu+sou+o+Vin%C3%ADcius;Infraestrutura+%2B+Automa%C3%A7%C3%A3o+%2B+Software+%2B+IA;Transformo+processos+manuais+em+sistemas" alt="Typing SVG" />

</div>

# Vinícius Bujes de Lima

**Automation Engineer · Full-Stack Developer · DevOps · AI**

Canoas, RS — Brasil &nbsp;·&nbsp; ProShows &nbsp;·&nbsp; Análise e Desenvolvimento de Sistemas — UNISINOS

---

### Meu diferencial

Transformo processos operacionais em sistemas confiáveis — conectando infraestrutura, automação, software, dados e IA. Parto da infraestrutura, automatizo o processo, desenvolvo o software quando necessário, estruturo os dados e aplico IA onde ela realmente agrega valor.

```
Infraestrutura
      ↓
  Automação
      ↓
  Software
      ↓
    Dados
      ↓
      IA
```

### Sobre mim

Construo automações com **N8N** para eliminar atrito operacional na ProShows e, quando a automação não basta, desenvolvo o sistema que falta — sustentado pela infraestrutura que também administro.

Aplico a mesma lógica no **Crônicas de Aethelgard**, meu laboratório pessoal, onde exploro arquitetura de software e IA aplicada, usando LLMs como componentes controlados do sistema — não como substitutos da lógica de negócio. No **AgentLab**, levo essa disciplina um passo além: construo a infraestrutura de engenharia para *avaliar* agentes de IA antes que eles cheguem à produção.

### Atualmente explorando

`AI Engineering` · `Agent Evaluation` · `Automation Engineering` · `Software Architecture` · `Data Engineering`

---

### Engenharia em prática

- **Framework de avaliação de agentes de IA** — [AgentLab](https://github.com/BujesL/AgentLab): motor de evaluation em Python que mede tool calling, reprodutibilidade e observabilidade de agentes de IA, com quality gates integrados a CI/CD. Segue Spec-Driven Development/OpenSpec de ponta a ponta (`spec.md` → `plan.md` → `contracts/` → `tasks.md`) — nenhuma feature relevante entra sem spec e contrato prévios. Um Provider Adapter desacopla o motor do LLM usado, evitando lock-in de fornecedor.
- **Service Desk com Spec-Driven Development** — [Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS): 4 features especificadas (`spec.md` → `plan.md` → `contracts/` → `tasks.md`) antes do código, ingestão de e-mail via Microsoft Graph, numeração de ticket atômica (`nextval()` na mesma transação, sem race condition), testes unit + integração.
- **Data pipeline em escala nacional** — [Startup Radar POA](https://github.com/BujesL/startup-radar-business-intelligence): filtra o dataset nacional de CNPJ (centenas de milhões de registros) com Polars em modo *lazy*, aplicando o recorte regional ainda no plano de execução, sem materializar a base inteira em memória.
- **Arquitetura de IA para produção** — no mesmo projeto, a Claude API só recebe dados já agregados pelo Postgres; nunca uma pergunta livre. O JSON usado fica salvo para auditoria. A decisão arquitetural é deliberada: a IA interpreta dados já validados; não define a verdade do sistema.
- **Automação em produção** — workflow N8N na ProShows integrando Outlook, Trello, Teams e SQL, com filtro de domínio corporativo contra chamados falsos.
- **Segurança desde o schema** — Row Level Security habilitado desde a criação das tabelas, escrita restrita a uma role que só o pipeline possui.

### Princípios de engenharia

- **Dados determinísticos antes da IA** — a IA interpreta dados já validados; não é fonte de verdade do sistema.
- **Segurança desde o design** — permissões, RLS e isolamento de acesso são definidos antes da aplicação existir.
- **Automação com controle** — workflows exigem validação, idempotência e rastreabilidade.
- **Software guiado por contratos** — features são especificadas antes da implementação e protegidas por testes.
- **IA não vai para produção sem avaliação** — agentes são medidos por métricas objetivas e quality gates antes de qualquer deploy.

---

### Stack

**Linguagens**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Backend & Dados**

![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

**Infra & Automação**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)

---

### Projetos em destaque

| Projeto | O que resolve | Engenharia | Stack |
|---|---|---|---|
| **[AgentLab](https://github.com/BujesL/AgentLab)** | Avalia sistematicamente agentes de IA (tool calling, reprodutibilidade, observabilidade) antes de irem para produção | Evaluation engine com métricas/traces/quality gates, Provider Adapter multi-LLM, Spec-Driven Development/OpenSpec, CI/CD | Python · Fastify · Next.js · PostgreSQL |
| **[Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS)** | Service desk interno: e-mail vira chamado rastreável | Spec-Driven Development, Microsoft Graph, numeração atômica, testes unit+integração | Fastify · PostgreSQL · React · N8N |
| **[Startup Radar POA](https://github.com/BujesL/startup-radar-business-intelligence)** | Identifica setores em crescimento na Grande Porto Alegre via CNPJ | Pipeline Polars lazy, agregados pré-computados, insight de IA auditável | Next.js 15 · Supabase · Polars |
| **[Cronicas-de-Aethelgard](https://github.com/BujesL/Cronicas-de-Aethelgard)** | TCG estilo Hearthstone (projeto pessoal) | Deck-building, keywords via event hooks, 6 facções | Flask · Python · JavaScript |
| **[Sultec-Bombas](https://github.com/BujesL/Sultec-Bombas)** | Modernização de site institucional | Layout responsivo, animações, lightbox | HTML · CSS · JavaScript |

---

### GitHub Stats

<div align="center">
  <img height="150" src="https://github-readme-stats-xi-five-29.vercel.app/api?username=BujesL&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
  <img height="150" src="https://github-readme-stats-xi-five-29.vercel.app/api/top-langs/?username=BujesL&layout=compact&theme=tokyonight&hide_border=true" />
</div>

---

### Contato

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vinicius.bujes04@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vinicius-bujes-465969245/)
