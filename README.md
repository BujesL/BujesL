<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&pause=1000&color=2E9EF7&center=true&vCenter=true&width=650&lines=Ol%C3%A1%2C+eu+sou+o+Vin%C3%ADcius;Infraestrutura+%2B+Automa%C3%A7%C3%A3o+%2B+Software+%2B+IA;Transformo+processos+manuais+em+sistemas" alt="Typing SVG" />

</div>

# Vinícius Bujes de Lima

**AI Automation Engineer · Full-Stack Software Engineer**

Canoas, RS — Brasil &nbsp;·&nbsp; ProShows &nbsp;·&nbsp; Análise e Desenvolvimento de Sistemas — UNISINOS

---

### Sobre mim

Conecto infraestrutura, automação, software, dados e IA para transformar processos operacionais manuais em sistemas confiáveis. Construo automações com **n8n** para eliminar atrito operacional na ProShows e, quando a automação não basta, desenvolvo o sistema que falta — sustentado pela infraestrutura que também administro.

```
Infraestrutura → Automação → Software → Dados → IA
```

No **AgentLab** — meu projeto principal no momento — levo essa disciplina para dentro da própria IA: construo a infraestrutura de engenharia para *avaliar* agentes antes que eles cheguem à produção. No **Crônicas de Aethelgard**, meu laboratório pessoal, aplico a mesma disciplina de engenharia migrando um protótipo Flask/Python para uma stack moderna (Next.js + TypeScript + Supabase), hoje em produção.

### Atualmente explorando

`AI Engineering` · `Agent Evaluation` · `Automation Engineering` · `Software Architecture` · `Data Engineering`

---

### Projeto em destaque: AgentLab

**Framework de avaliação de agentes de IA** — [AgentLab](https://github.com/BujesL/AgentLab): motor de avaliação em Python que mede tool calling, reprodutibilidade e observabilidade de agentes de IA, com quality gates integrados a CI/CD. Segue Spec-Driven Development/OpenSpec de ponta a ponta (`spec.md` → `plan.md` → `contracts/` → `tasks.md`) — nenhuma feature relevante entra sem spec e contrato prévios. Um Provider Adapter desacopla o motor do LLM usado, evitando lock-in de fornecedor.

### Engenharia em prática

- **Service Desk com Spec-Driven Development** — [Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS): e-mail vira chamado rastreável via Microsoft Graph, numeração sequencial via `nextval()` na mesma query de INSERT (elimina a race condition clássica de ler-e-incrementar em duas etapas), deduplicação por `source_message_id`, 4 features especificadas com Spec-Driven Development antes do código.
- **Data pipeline em escala nacional** — [Startup Radar POA](https://github.com/BujesL/startup-radar-business-intelligence): filtra o cadastro nacional de CNPJ da Receita Federal (centenas de milhões de registros) com Polars em modo *lazy* — predicate pushdown aplica o recorte regional ainda no plano de execução, sem materializar a base inteira em memória. Carga em Postgres via `COPY`, não `INSERT` linha a linha.
- **IA como componente auditável, não fonte de verdade** — no mesmo projeto, a Claude API só recebe o JSON já agregado pelo Postgres; nunca uma pergunta livre sobre o dataset bruto. O JSON usado fica salvo junto ao insight gerado, então qualquer frase da IA é rastreável até o número exato que a originou.
- **Migração de protótipo para produção** — [Crônicas de Aethelgard](https://github.com/BujesL/Cronicas-de-Aethelgard): jogo de cartas 1v1 contra IA, migrado de um protótipo Flask/JavaScript puro para Next.js 16 + TypeScript + Supabase (Auth, Postgres, RLS), em produção na Vercel.
- **Automação em produção** — workflow n8n que processa chamados recebidos por e-mail, classifica solicitações e integra Outlook, Teams, Trello e SQL, reduzindo etapas manuais do atendimento.
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

**Backend & Dados**

![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

**AI & Automation**

![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)

**Infra & DevOps**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

### Projetos em destaque

| Projeto | O que resolve | Engenharia | Stack |
|---|---|---|---|
| **[AgentLab](https://github.com/BujesL/AgentLab)** | Avalia sistematicamente agentes de IA (tool calling, reprodutibilidade, observabilidade) antes de irem para produção | Engine de avaliação com métricas/traces/quality gates, Provider Adapter desacoplado, atualmente com providers Mock e Ollama e preparado para integração com outros LLMs, Spec-Driven Development/OpenSpec, CI/CD | Python · Fastify · Next.js · PostgreSQL |
| **[Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS)** | Service desk interno: e-mail vira chamado rastreável | Spec-Driven Development, Microsoft Graph, numeração atômica via `nextval()`, testes unit+integração (Vitest) | Fastify · PostgreSQL · React · Microsoft Graph |
| **[Startup Radar POA](https://github.com/BujesL/startup-radar-business-intelligence)** | Identifica setores em crescimento na Grande Porto Alegre a partir do cadastro nacional de CNPJ | Pipeline Polars lazy (predicate pushdown), carga via `COPY`, agregados pré-computados, RLS desde o schema, insight de IA auditável | Next.js 15 · Supabase · Polars |
| **[Cronicas-de-Aethelgard](https://github.com/BujesL/Cronicas-de-Aethelgard)** | Jogo de cartas 1v1 contra IA — protótipo Flask migrado para produção | Migração completa de arquitetura, Auth + RLS via Supabase, deploy contínuo na Vercel | Next.js 16 · React 19 · TypeScript · Supabase |
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
