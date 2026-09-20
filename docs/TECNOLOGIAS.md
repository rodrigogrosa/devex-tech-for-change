# Tecnologias, linguagens e frameworks

[← Voltar ao README](../README.md)

Esta relação foi preparada a partir dos manifestos e da organização da implementação disponibilizada pelo responsável pelo projeto. Ela descreve a base técnica consultada; não é um inventário extraído do servidor em execução.

## Frontend

| Tecnologia | Referência declarada | Uso |
|---|---|---|
| TypeScript | Linha 5.7 | Tipagem da interface e contratos no cliente |
| React | Linha 19 | Componentes da aplicação web |
| Vite | Linha 6 | Desenvolvimento e build da interface |
| Tailwind CSS | Linha 4 | Estilos e composição visual |
| Radix UI | Dependências por componente | Componentes de interação |
| TanStack Query | Linha 5 | Gerenciamento de dados remotos |
| Zustand | Linha 5 | Estado de interface |
| React Hook Form e Zod | Linhas 7 e 3 | Formulários e validação |
| React Flow e Dagre | Bibliotecas declaradas | Visualização e organização de fluxos |
| Mermaid | Linha 11 | Diagramas |
| Vitest e Playwright | Dependências de desenvolvimento | Testes de componentes e ponta a ponta |

O manifesto declara Node.js 22.22 ou superior como requisito de ambiente do frontend. Intervalos de dependência não equivalem às versões efetivamente resolvidas por um arquivo de lock.

## Backend e dados

| Tecnologia | Referência declarada | Uso |
|---|---|---|
| Python | 3.12 ou superior | Linguagem do backend |
| FastAPI | 0.139.2 | API HTTP |
| Uvicorn | 0.49.0 | Servidor ASGI |
| Pydantic | 2.13.4 | Schemas e validação |
| SQLAlchemy | 2.0.31 | Persistência e acesso aos dados |
| asyncpg | 0.29.0 | Conexão assíncrona ao PostgreSQL |
| Alembic | 1.13.2 | Migrações de schema |
| PostgreSQL | Imagem 16-alpine | Banco relacional |
| Redis | Imagem 7-alpine | Cache e mecanismos auxiliares |
| HTTPX | 0.28.1 | Comunicação HTTP |
| PyJWT, bcrypt e pyotp | Dependências declaradas | Mecanismos de autenticação e proteção de credenciais |

## Inteligência artificial e conhecimento

| Tecnologia | Referência declarada | Responsabilidade |
|---|---|---|
| LiteLLM | 1.88.0 | Gateway de acesso a modelos |
| LangChain | 1.3.14 | Composição de integrações e fluxos de IA |
| LangGraph | 1.2.9 | Orquestração com estado |
| Claude Agent SDK | 0.2.143 | Fluxos de agentes com ferramentas |
| Graphify / graphifyy | 0.9.8 | Conhecimento e análise do repositório |
| NetworkX | 3.6.1 | Estruturas e análise de grafos |
| Langfuse | SDK 2.60.10 | Observabilidade da execução de IA |
| DeepEval e Ragas | Dependências declaradas | Recursos para avaliação de fluxos de IA |

A disponibilidade de modelos e provedores depende das credenciais, configurações e políticas do ambiente. A presença de bibliotecas de avaliação não comprova a execução de uma campanha de avaliação nem seus resultados.

## Operação e qualidade

- **Docker e Docker Compose:** empacotamento e composição dos serviços.
- **Nginx:** entrega do frontend e encaminhamento para a API.
- **OpenTelemetry:** instrumentação de serviços e exportação de telemetria.
- **Prometheus e Grafana:** métricas e painéis, conforme perfil habilitado.
- **Pytest:** testes da implementação Python.
- **Ruff, mypy, Bandit e pip-audit:** verificações estáticas e de dependências declaradas na base técnica.
- **Vitest, Testing Library e Playwright:** ferramentas declaradas para testes da interface.

## Rastreabilidade da leitura

As referências consultadas foram `pyproject.toml`, `requirements.txt`, `frontend/package.json`, `docker-compose.yml`, o cliente de LiteLLM e módulos de conhecimento do código e de operação.

Esses caminhos identificam a origem técnica da documentação na implementação mantida separadamente. Não são links para arquivos deste repositório e não implicam publicação do código privado.
