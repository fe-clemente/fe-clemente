<div align="center">

# Fernando Clemente
### Engenheiro de IA · Full Stack · IA generativa em produção

Projeto, desenvolvo e opero de ponta a ponta o ecossistema de sistemas de uma rede de franquias de alimentação, com IA embarcada para usuários, gestão e franqueados. Hoje atende mais de 280 lojas no Brasil.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-clementeads-A73C21?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/clementeads)
![Open to work](https://img.shields.io/badge/aberto_a-novas_oportunidades-FF0E22?style=flat-square)

</div>

---

## Resultados medidos

| Entrega | Antes | Depois |
|---|---|---|
| Extração de dados de documentos de pagamento com IA | 94% de acerto | **98%** (99,7% em guias de imposto), em 148 documentos reais |
| Relatório de CMV por loja | 241 s | **6 s** (~40x), validado em 144 casos |
| Vendas da rede, de vários PDVs | relatórios separados por sistema | **base única desde 2018**, 99,9% de aderência à base oficial |
| Extrato bancário no ERP | importação manual | **API bancária**, 100% das execuções sem intervenção, 0 duplicados |
| NF-e de compra | digitação | **40%** entram direto via SEFAZ |
| Vazão de entregas | 98 por mês | **213 por mês** (+117%) |

---

## Ecossistema

<img width="2400" height="1100" alt="Telas dos sistemas, com marcas preservadas" src="https://github.com/user-attachments/assets/24f57a55-4790-404f-91f1-b296ae308b85" />
<img width="2951" height="1150" alt="Mapa do ecossistema" src="https://github.com/user-attachments/assets/4ef611e3-881d-485e-80f9-2f7ed434a2aa" />

Criei todos os sistemas do mapa. O núcleo, em números:

| | |
|---|---|
| **97** módulos | **680** páginas |
| **1.628** services | **580** tabelas |
| **270** agentes de IA | **6.446** nós mapeados |
| **8.752** commits | **237** dias no ar |
| **25+** integrações homologadas via API e MCP | |

Integrações com iFood, Keeta, Latam, ERPs, middleware bancário, AWS, Claude, Codex, Gemini e mais. Também refatorei por completo e hoje faço a gestão de outros sistemas que não aparecem no mapa.

O mapa mostra a estrutura, não o conteúdo.

---

## Como eu trabalho com IA

- **LLM como componente, não como orquestrador.** A automação é determinística e versionada. O modelo é chamado de forma explícita, onde agrega, com entrada e saída controladas.
- **Agentes em produção.** Motor próprio de agentes com agendamento, execução auditada, logs e painel em tempo real.
- **RAG sobre base própria.** Busca semântica com PostgreSQL + pgvector, com centenas de fontes internas indexadas.
- **Modelo escolhido com medição.** Claude, Gemini, Groq e Codex, cada um onde faz sentido. Antes de ir para produção, comparo variantes no mesmo roteiro de teste, com custo e qualidade medidos.
- **Assistente embarcado.** Widget de IA presente nas páginas dos sistemas, com contexto do módulo em uso.
- **Engenharia com agentes de código.** Spec-Driven Development com Claude Code: contexto versionado em repositório, skills por domínio, subagentes de revisão e QA, e revisão humana antes de ir ao ar.
- **Segurança desde o desenho.** RBAC, isolamento multi-inquilino, trilha de auditoria, ambiente de homologação com envios bloqueados e rotinas automatizadas de verificação de segurança.

---

## Stack

**IA:** Claude · Gemini · Groq · Codex · MCP · RAG · agentes  
**Back-end:** Node.js · Express · PHP 8 · Laravel  
**Dados:** MySQL · PostgreSQL · pgvector · Redis  
**Infra:** Linux · PM2 · Docker · AWS (S3, CodeDeploy) · Apache  
**Front:** HTML/CSS/JS · Blade · Tailwind · mobile-first  
**Integrações:** WhatsApp Cloud API · Google Workspace · marketplaces de delivery · ERPs · bancos · SEFAZ

---

## Por que não tem código aqui

São sistemas proprietários da empresa, não projetos pessoais. Por isso não publico código, dados, regras de negócio nem detalhes internos.

Sobre arquitetura e decisões técnicas, falo com prazer. Me chama no [LinkedIn](https://www.linkedin.com/in/clementeads).
