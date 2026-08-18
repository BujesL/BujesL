<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&pause=1000&color=2E9EF7&center=true&vCenter=true&width=650&lines=Ol%C3%A1%2C+eu+sou+o+Vin%C3%ADcius;Infraestrutura+%2B+Automa%C3%A7%C3%A3o+%2B+Dev+%2B+IA;Transformo+processos+manuais+em+sistemas" alt="Typing SVG" />

</div>

# Vinícius Bujes de Lima

**AI Automation Engineer · Full-Stack Developer · DevOps**

Canoas, RS — Brasil &nbsp;·&nbsp; ProShows &nbsp;·&nbsp; Análise e Desenvolvimento de Sistemas — UNISINOS

---

### 🧩 Meu diferencial

Não sou só "quem sabe Python" ou "quem sabe Next.js" — o que faço de fato é fechar o ciclo completo de um problema operacional real:

```
Infraestrutura → Automação → Desenvolvimento → Dados → IA
```

Na prática: administro os servidores e a telefonia onde o problema mora, construo a automação que resolve a dor imediata, desenvolvo o sistema quando a automação não é suficiente, modelo os dados que sustentam esse sistema, e uso IA para extrair sinal desses dados — sem que a IA nunca vire a fonte da verdade (mais sobre isso nos destaques abaixo).

É essa combinação — não uma linguagem isolada — que estrutura como eu resolvo problema.

### Sobre mim

Atuo na **ProShows** com um perfil híbrido de **infraestrutura, automação e desenvolvimento**: administro servidores, sistemas de telefonia Avaya e racks, construo **automações de processo com N8N** (Outlook, Trello, Teams, SQL) e desenvolvo aplicações full-stack para necessidades internas da empresa.

Fora do trabalho, mantenho o **Crônicas de Aethelgard**, um TCG (jogo de cartas) inspirado em Hearthstone, com backend em Flask/Python e frontend em HTML/CSS/JS.

Uso IA (Claude, GitHub Copilot) como copiloto de desenvolvimento no dia a dia, tanto em automações corporativas quanto em projetos pessoais.

### 🎯 Foco atual

- Modernizando o site institucional da Sultec Bombas com uma abordagem Spec-Driven Development
- Evoluindo o sistema de cartas do Crônicas de Aethelgard (novo sistema de energia e keywords)
- Aprofundando em arquitetura de automações N8N e integrações via API

---

### 📈 Destaques técnicos

Evidência concreta por trás dos projetos — o tipo de decisão que não aparece só lendo o nome da stack:

- **Pipeline de dados em escala nacional, filtrado para uso regional** — no [radarPOA](https://github.com/BujesL/radarPOA), processo o cadastro de CNPJ da Receita Federal (centenas de milhões de registros) com Polars em modo *lazy* (`scan_csv`), aplicando o filtro regional ainda no plano de execução — nunca materializando o dataset nacional inteiro em memória.
- **IA sem alucinação por design** — no mesmo projeto, a Claude API nunca recebe uma pergunta livre sobre os dados: ela só recebe o JSON já agregado pelo Postgres e sua única tarefa é narrar esse JSON. O JSON usado fica salvo para auditoria — qualquer frase gerada pode ser checada contra o número exato que a originou.
- **Sistema de service desk com Spec-Driven Development completo** — o [Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS) tem 4 features com especificação formal (`spec.md` → `plan.md` → `contracts/` → `tasks.md`) escritas **antes** do código, ingestão automática de e-mail via Microsoft Graph com numeração de chamado atômica (`nextval()` na mesma transação, sem race condition), e suíte de testes unitários + integração.
- **Automação de produção com filtro anti-spam** — workflow N8N em produção na ProShows que integra Outlook, Trello, Teams e SQL, com filtro de domínio corporativo para impedir que e-mails externos gerem chamados falsos no sistema interno.
- **Segurança desde o schema, não como retrofit** — Row Level Security habilitado desde a criação das tabelas (não adicionado depois), com escrita restrita a uma role que só o pipeline possui — o frontend nunca tem permissão de alterar dados.

---

### 🛠️ Stack & Ferramentas

**Linguagens**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Backend & Frameworks**

![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)

**Frontend**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

**Banco de Dados**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

**Infra, Cloud & DevOps**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Windows Server](https://img.shields.io/badge/Windows_Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)

**Automação, ERP & IA**

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Protheus](https://img.shields.io/badge/Protheus-ERP-FF6600?style=for-the-badge)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)

---

### Projetos em destaque

| Projeto | O que resolve | Complexidade real | Stack |
|---|---|---|---|
| **[Sistema-de-Chamados-PS](https://github.com/BujesL/Sistema-de-Chamados-PS)** | Service desk interno: e-mail vira chamado rastreável automaticamente | Monorepo com Spec-Driven Development, ingestão via Microsoft Graph, numeração atômica, testes unit+integração | Fastify · PostgreSQL · React · N8N |
| **[radarPOA](https://github.com/BujesL/radarPOA)** | Identifica setores em crescimento na Grande Porto Alegre a partir do cadastro nacional de CNPJ | Pipeline que filtra centenas de milhões de registros sem carregar tudo em memória; insight de IA auditável | Next.js 15 · Supabase · Polars |
| **[Cronicas-de-Aethelgard](https://github.com/BujesL/Cronicas-de-Aethelgard)** | TCG estilo Hearthstone (projeto pessoal) | Sistema de energia, deck-building, keywords via event hooks (Battlecry, Deathrattle, Taunt), 6 facções | Flask · Python · JavaScript |
| **[Sultec-Bombas](https://github.com/BujesL/Sultec-Bombas)** | Modernização de site institucional | Layout responsivo, animações, lightbox, menu mobile | HTML · CSS · JavaScript |
| **[clone-yu-gi-oh](https://github.com/BujesL/clone-yu-gi-oh)** | Estudo de interface de jogo de cartas | Embrião que originou o Crônicas de Aethelgard | HTML · JavaScript |

---

### GitHub Stats

<div align="center">
  <img height="165" src="https://github-readme-stats-xi-five-29.vercel.app/api?username=BujesL&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats-xi-five-29.vercel.app/api/top-langs/?username=BujesL&layout=compact&theme=tokyonight&hide_border=true" />
</div>


---

### Contato

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vinicius.bujes04@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vinicius-bujes-465969245/)
