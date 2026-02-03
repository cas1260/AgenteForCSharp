# Agents CSharp

Repositório de agentes especializados da SwapSoft para software houses, orientado à Stack Microsoft (.NET 8, Azure, Azure DevOps e Azure AD). Cada agente cobre uma área do ciclo de vida do software, do discovery à entrega, com foco em qualidade, segurança e disciplina de escopo.

## Como usar (por editor/LLM)

### Trae IDE
- Crie agentes no painel de criação de agentes e copie o conteúdo dos arquivos deste repositório como prompt do agente.
- Use @ no chat para selecionar o agente criado e executar tarefas específicas.

### Cursor AI
- Use agentes para tarefas com objetivo claro e delegue o trabalho via chat.
- Uma prática comum é manter instruções de agentes em arquivos Markdown e referenciá-los com @arquivo no prompt.

### VS Code (GitHub Copilot)
- Crie agentes customizados em arquivos .agent.md e coloque em .github/agents para aparecerem no seletor de agentes.
- Use .github/copilot-instructions.md e/ou AGENTS.md para instruções globais ou por pasta.

### Claude Code
- Crie subagents em .claude/agents ou ~/.claude/agents, usando Markdown com frontmatter.
- Use /agents para gerenciar, editar e ativar subagents.

### Google Gemini (Code Assist)
- Use o modo Agent no Gemini Code Assist e forneça contexto persistente com arquivos GEMINI.md.
- No Android Studio, use AGENTS.md para instruções específicas por diretório.

### Google Antigravity
- Use o Agent Manager para despachar tarefas a agentes e acompanhar Artifacts.
- Organize instruções como Rules/Workflows/Skills e carregue as definições dos agentes nesses artefatos.
- Opcional: use .antigravity/rules.md como ponto central de regras do repositório.

### Gemini CLI
- Crie um arquivo GEMINI.md na raiz do repositório para contexto persistente nas execuções via terminal.

## Resumo de Regras e Equipe

- Escopo absoluto: executar somente o que foi solicitado, sem extras.
- Gatilho obrigatório: somente após “faça sua mágica” é permitido alterar arquivos.
- Sem suposições: se faltar informação essencial, perguntar o mínimo necessário.
- Edição mínima: preservar padrões, arquitetura e convenções existentes.
- Banco de dados: apenas SELECT; alterações são entregues como script.
- Sem remoções: nenhum arquivo é apagado sem confirmação explícita.
- Dados reais: nunca usar mock; preferir dados do projeto.
- Dependências: não adicionar bibliotecas novas.
- Checklist obrigatório: checklist.txt é fonte única de verdade e deve ser atualizado.
- Idioma: todo o conteúdo em Português do Brasil.
- Validação rigorosa: confirmar tudo antes de finalizar.
- Equipe: Frank (gestão), Prime (análise/planejamento), especialistas por stack, revisão obrigatória e validação final por Neo.

## Agentes

- backend-specialist.md -> Agente focado em backend .NET/Azure para APIs, lógica de servidor, integrações e segurança.
- code-archaeologist.md -> Agente focado em legado, refatoração segura, entendimento e modernização de código.
- database-architect.md -> Agente focado em modelagem, schema, queries, migrations e decisão entre Azure SQL/Cosmos DB.
- debugger.md -> Agente focado em investigação de bugs, análise de causa raiz e correções verificáveis.
- devops-engineer.md -> Agente focado em deploy, CI/CD, operações, rollback e monitoramento em produção.
- documentation-writer.md -> Agente focado em documentação técnica (README, API docs, changelog).
- explorer-agent.md -> Agente focado em descoberta de codebase, mapeamento arquitetural e pesquisa de viabilidade.
- frontend-specialist.md -> Agente focado em UI .NET (Blazor/ASP.NET Core/Fluent UI), UX, responsividade e padrões de front.
- game-developer.md -> Agente focado em desenvolvimento de jogos com DirectX, Xbox GDK e PlayFab.
- mobile-developer.md -> Agente focado em apps .NET MAUI, padrões mobile, performance e UX multiplataforma.
- orchestrator.md -> Agente focado em coordenação multiagente e orquestração de tarefas complexas.
- penetration-tester.md -> Agente focado em pentest, simulação de ataques e validação de vulnerabilidades.
- performance-optimizer.md -> Agente focado em profiling e otimização de performance e estabilidade.
- product-manager.md -> Agente focado em requisitos, user stories, critérios de aceite e priorização.
- project-planner.md -> Agente focado em planejamento, decomposição de tarefas e dependências.
- qa-automation-engineer.md -> Agente focado em automação E2E com Playwright e pipelines de testes.
- security-auditor.md -> Agente focado em auditoria de segurança, OWASP e supply chain.
- seo-specialist.md -> Agente focado em SEO/GEO, Core Web Vitals e visibilidade em busca.
- test-engineer.md -> Agente focado em testes unitários, integração, E2E e TDD.

## Referências

- https://docs.trae.ai/ide/agent
- https://cursor.com/learn/agents
- https://www.chatprd.ai/how-i-ai/workflows/how-to-create-a-reusable-ai-agent-in-cursor-for-consistent-document-generation
- https://code.visualstudio.com/docs/copilot/customization/custom-agents
- https://code.visualstudio.com/docs/copilot/customization/custom-instructions
- https://code.claude.com/docs/en/sub-agents
- https://developers.google.com/gemini-code-assist/docs/use-agentic-chat-pair-programmer
- https://developer.android.com/studio/gemini/agent-files
- https://codelabs.developers.google.com/getting-started-google-antigravity
- https://github.com/study8677/antigravity-workspace-template
- https://github.com/google-gemini/gemini-cli
