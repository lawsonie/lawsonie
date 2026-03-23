# Lawson · Portfólio de Desenvolvimento Assistido por IA
### *From Zero to Product — A PM's Journey Through AI-Assisted Development*

---

> **PT** | [EN below](#english-version)

---

## 🇧🇷 Versão em Português

### Quem sou

Sou Lawson, profissional em transição de carreira do Direito para Gestão de Produto e Tecnologia. Tenho formação jurídica com TCC em LGPD, o que me deu uma perspectiva diferenciada sobre privacidade de dados aplicada a sistemas reais. Hoje estudo e pratico Product Management e Product Owner usando metodologias ágeis (Scrumban/Jira) em projetos reais que eu mesmo construo e coordeno com assistência de IA.

Não tenho formação técnica tradicional em programação. **Aprendo por engenharia reversa**: estudo o código gerado pela IA, submeto a análises, identifico padrões, e coordeno o desenvolvimento como um PM que entende profundamente a stack que supervisiona.

---

### A Jornada em 3 Fases

Este portfólio documenta uma progressão real, sem cortes — de total curiosidade até coordenação de produto com stack profissional.

---

#### ⚡ Fase 0 — `lawsonia_alpha`
**Inteligência Jurídica e Institucional · Python + Streamlit + Gemini API**
> *"No primeiro ou segundo dia, eu só queria ver funcionar."*

O ponto de partida. Usei meu domínio jurídico como objeto de teste para explorar o que era possível construir com IA.

**O que foi entregue:**
- Sistema com deploy em produção (Streamlit Cloud), acessível remotamente
- Autenticação com sessão persistente via cookies (CookieManager + React assíncrono)
- Integração real com Gemini API para consultas jurídicas
- Leitura e análise de documentos PDF e DOCX
- Módulo de prazos jurídicos (`prazos_data.py`) com regras de tempestividade
- Preparação para Supabase Auth (importação condicional, variáveis de ambiente com fallback)
- Design visual próprio: identidade "tech authority" com tipografia Space Grotesk, gradiente ciano/azul, efeito glow

**O que aprendi:**
- Limitações do Streamlit para sessões multi-usuário
- O problema estrutural de cookies assíncronos em frameworks de UI declarativa
- Como secrets funcionam entre ambiente local (`.env`) e cloud (Streamlit secrets)
- Que design de identidade visual é uma decisão estratégica, não decoração

**Stack:** Python · Streamlit · Gemini API · PyPDF2 · python-docx · Supabase (prep) · extra-streamlit-components

---

#### 🏗️ Fase 1 — `somente-python`
**Sistema de Gestão para Consultório · Python + Streamlit + Gemini API**
> *"Agora com um problema real, usuário real, e disciplina de projeto."*

Migração do aprendizado para um produto funcional com propósito claro: sistema de gestão para consultório médico/terapêutico real. Não era mais curiosidade — era entrega.

**O que foi entregue:**
- Arquitetura em camadas bem definidas: `auth/`, `services/`, `database/`, `data/`
- Sistema de autenticação com banco de dados (`auth.py` + `auth_db.py`) separados por responsabilidade
- Integração de IA com restrições controladas de framework (limites de contexto, guardrails)
- Repositório contábil com dados reais (`repositorio_contabil/02-2025`)
- `teste_api.py` separado — validação de integração antes de incorporar ao produto
- `app_backup_ui.py` — gestão de risco: backup de versão anterior antes de refatorar

**O que aprendi:**
- Separação de responsabilidades (o `services/` como camada de negócio)
- Como banco de dados persiste estado entre sessões
- Que testar integração de API isoladamente antes de integrar ao produto é prática correta
- Gestão de versão pragmática mesmo sem dominar Git completamente

**Stack:** Python · Streamlit · Gemini API · SQLite · python-dotenv

---

#### 🚀 Fase 2 — `espaco-somente-web` *(em desenvolvimento)*
**Sistema de Gestão para Consultório · Next.js + TypeScript + Tailwind + shadcn/ui**
> *"Stack profissional, metodologia real, produto escalável."*

Reescrita completa em stack moderna, coordenada como projeto de produto com metodologia Scrumban no Jira. O `somente-python` funciona como especificação funcional — cada módulo Python mapeado para seu equivalente Next.js.

**O que está sendo construído:**
- App Router (Next.js 14+) com TypeScript rigoroso
- Autenticação via `middleware.ts` com proteção de rotas
- Componentes reutilizáveis com shadcn/ui + Tailwind CSS
- Arquitetura: `app/` (páginas) · `components/` · `hooks/` · `lib/` (integrações, db)
- Integração de IA planejada: Gemini API (fase de desenvolvimento) → Claude API (produção)
- Gerenciamento com OpenSquad (framework multi-agente) + Antigravity IDE

**Por que a migração faz sentido:**
- Next.js escala para múltiplos usuários simultâneos (Streamlit não)
- TypeScript força precisão na modelagem de dados — aprendo estrutura enquanto construo
- shadcn/ui entrega componentes acessíveis e de qualidade profissional
- A stack abre caminho para vender ou licenciar o produto para outros consultórios

**Metodologia de projeto:**
- Scrumban no Jira como treino de PM/PO
- OpenSquad com Gemini API como motor de agentes (sem custo durante desenvolvimento)
- Claude como assistente de revisão, arquitetura e coordenação de produto

**Stack:** Next.js · TypeScript · React · Tailwind CSS · shadcn/ui · Node.js · pnpm · Gemini API · (Claude API planejado)

---

### Por que este portfólio importa

A maioria dos portfólios mostra o produto final. Este mostra **o processo de quem aprendeu construindo**.

Cada decisão está documentada. Cada limitação encontrada virou aprendizado registrado. Cada fase tem um "antes e depois" claro. Isso é o que um PM faz: entende o sistema profundamente o suficiente para coordenar seu desenvolvimento, mesmo sem executar cada linha de código.

O background jurídico não é um desvio — é um diferencial. Sistemas que lidam com dados de saúde, documentos de clientes e informações sensíveis precisam de alguém que entenda LGPD não como checklist, mas como princípio de design.

---

### Próximos passos

- [ ] Completar módulos core do `espaco-somente-web` (agendamentos, prontuários, financeiro)
- [ ] Integrar IA ao sistema (triagem de formulários, lembretes automatizados)
- [ ] Deploy do sistema Next.js para o consultório real
- [ ] Documentar os squads OpenSquad usados no desenvolvimento
- [ ] Publicar template de sistema para pequenos consultórios/escritórios

---

### Contato

**GitHub:** [@lawsonie](https://github.com/lawsonie)

---
---

## 🇺🇸 English Version {#english-version}

### Who I am

I'm Lawson, a career-transition professional moving from Law to Product Management and Technology. My legal background includes a thesis on Brazil's data protection law (LGPD), which gives me a distinct perspective on privacy-by-design applied to real systems. Today I study and practice Product Management and Product Owner roles using agile methodologies (Scrumban/Jira) on real projects I build and coordinate with AI assistance.

I have no traditional programming background. **I learn through reverse engineering**: I study AI-generated code, submit it to analysis, identify patterns, and coordinate development as a PM who deeply understands the stack he supervises.

---

### The Journey in 3 Phases

This portfolio documents a real progression, uncut — from pure curiosity to product coordination with a professional stack.

---

#### ⚡ Phase 0 — `lawsonia_alpha`
**Legal & Institutional Intelligence System · Python + Streamlit + Gemini API**
> *"On day one or two, I just wanted to see it work."*

The starting point. I used my legal domain expertise as a test object to explore what was possible to build with AI.

**What was delivered:**
- System deployed to production (Streamlit Cloud), accessible remotely
- Authentication with persistent sessions via cookies (async React CookieManager)
- Real Gemini API integration for legal queries
- PDF and DOCX document reading and analysis
- Legal deadlines module (`prazos_data.py`) with procedural timing rules
- Supabase Auth preparation (conditional imports, env variable fallback)
- Custom visual identity: "tech authority" design with Space Grotesk typography, cyan/blue gradient, glow effects

**What I learned:**
- Streamlit's limitations for multi-user sessions
- The structural problem of async cookies in declarative UI frameworks
- How secrets work between local (`.env`) and cloud (Streamlit secrets) environments
- That visual identity design is a strategic decision, not decoration

**Stack:** Python · Streamlit · Gemini API · PyPDF2 · python-docx · Supabase (prep) · extra-streamlit-components

---

#### 🏗️ Phase 1 — `somente-python`
**Clinic Management System · Python + Streamlit + Gemini API**
> *"Now with a real problem, a real user, and project discipline."*

Transition from learning to a functional product with clear purpose: management system for a real medical/therapeutic clinic. No longer curiosity — this was delivery.

**What was delivered:**
- Well-defined layered architecture: `auth/`, `services/`, `database/`, `data/`
- Database-backed authentication (`auth.py` + `auth_db.py`) with separated responsibilities
- AI integration with controlled framework restrictions (context limits, guardrails)
- Accounting repository with real data (`repositorio_contabil/02-2025`)
- Isolated `teste_api.py` — API validation before product integration
- `app_backup_ui.py` — risk management: version backup before refactoring

**What I learned:**
- Separation of concerns (`services/` as the business logic layer)
- How databases persist state across sessions
- That testing API integration in isolation before merging is correct practice
- Pragmatic version management even without mastering Git fully

**Stack:** Python · Streamlit · Gemini API · SQLite · python-dotenv

---

#### 🚀 Phase 2 — `espaco-somente-web` *(in development)*
**Clinic Management System · Next.js + TypeScript + Tailwind + shadcn/ui**
> *"Professional stack, real methodology, scalable product."*

Complete rewrite in modern stack, coordinated as a product project with Scrumban methodology on Jira. The `somente-python` project serves as functional specification — each Python module mapped to its Next.js equivalent.

**What is being built:**
- Next.js 14+ App Router with strict TypeScript
- Route protection via `middleware.ts`
- Reusable components with shadcn/ui + Tailwind CSS
- Architecture: `app/` (pages) · `components/` · `hooks/` · `lib/` (integrations, db)
- AI integration planned: Gemini API (development phase) → Claude API (production)
- Managed with OpenSquad (multi-agent framework) + Antigravity IDE

**Why the migration makes sense:**
- Next.js scales for concurrent users (Streamlit doesn't)
- TypeScript enforces data modeling precision — I learn structure while building
- shadcn/ui delivers accessible, production-quality components
- The stack opens a path to sell or license the product to other clinics

**Project methodology:**
- Scrumban on Jira as PM/PO training
- OpenSquad with Gemini API as agent engine (zero cost during development)
- Claude as review assistant, architecture advisor, and product coordination

**Stack:** Next.js · TypeScript · React · Tailwind CSS · shadcn/ui · Node.js · pnpm · Gemini API · (Claude API planned)

---

### Why this portfolio matters

Most portfolios show the final product. This one shows **the process of someone who learned by building**.

Every decision is documented. Every limitation encountered became a recorded lesson. Each phase has a clear before and after. That's what a PM does: understands the system deeply enough to coordinate its development, even without writing every line of code.

The legal background isn't a detour — it's a differentiator. Systems handling health data, client documents, and sensitive information need someone who understands data protection law not as a checklist, but as a design principle.

---

### Next Steps

- [ ] Complete core modules of `espaco-somente-web` (scheduling, records, financials)
- [ ] Integrate AI into the system (form triage, automated reminders)
- [ ] Deploy Next.js system to the real clinic
- [ ] Document the OpenSquad squads used in development
- [ ] Publish a template system for small clinics and service offices

---

### Contact

**GitHub:** [@lawsonie](https://github.com/lawsonie)
