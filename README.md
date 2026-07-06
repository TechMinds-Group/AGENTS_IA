# AGENTS_IA

> Pacote [Agent Companies](https://agentcompanies.io) (`agentcompanies/v1`) com os 59 agentes da Arquitetura V6 do [Paperclip-Organization](https://github.com/TechMinds-Group), coordenados via [Paperclip](https://github.com/paperclipai/paperclip) e executados via OpenCode (`opencode_local`).

Skills utilizadas: 91, do catálogo [SKILLS_AI](https://github.com/TechMinds-Group/SKILLS_AI) (mesma organização).

## Estrutura

```
AGENTS_IA/
├── COMPANY.md
├── teams/
│   ├── governanca-ceo/TEAM.md          # 6 agentes
│   ├── produto-engenharia/TEAM.md      # 27 agentes
│   ├── revenue/TEAM.md                 # 15 agentes
│   └── financas-compliance/TEAM.md     # 11 agentes
├── agents/
│   └── <slug>/
│       ├── AGENTS.md      # camada de pacote (agentcompanies/v1)
│       ├── HEARTBEAT.md   # camada de runtime
│       ├── SOUL.md        # camada de runtime
│       └── TOOLS.md       # camada de runtime
└── .paperclip.yaml         # adapter opencode_local por agente
```

## Inventário completo (59 agentes)

| # | Agente | Tipo | Tier | Reporta a | Heartbeat | Priority |
|---|--------|------|------|-----------|-----------|----------|
| 1 | CEO | Core | 1 | — | Semanal | critical |
| 2 | Chief of Staff | Core | 2 | CEO | Diário | high |
| 3 | Knowledge Manager | Core | 2 | CEO | Semanal | high |
| 4 | COO | Core | 2 | CEO | Diário | high |
| 5 | AgentOps Agent | Reactive | 5 | COO | Diário | medium |
| 6 | Process Agent | Specialist | 3 | COO | Sob demanda | medium |
| 7 | Product & Engineering Director | Core | 2 | CEO | Semanal | critical |
| 8 | Product Manager Agent | Core | 2 | Product & Engineering Director | Diário | high |
| 9 | Roadmap Agent | Specialist | 3 | Product Manager Agent | Sob demanda | medium |
| 10 | Competitor Intel Agent | Specialist | 5 | Product Manager Agent | Quinzenal | low |
| 11 | Pricing Agent | Specialist | 2 | Product Manager Agent | Mensal | high |
| 12 | Localization Agent | Specialist | 5 | Product Manager Agent | Sob demanda | low |
| 13 | UX Design Agent | Specialist | 2 | Product & Engineering Director | Sob demanda | high |
| 14 | UX Research Agent | Specialist | 3 | UX Design Agent | Sob demanda | medium |
| 15 | Design System Agent | Specialist | 3 | UX Design Agent | Sob demanda | medium |
| 16 | Creative Design Agent | Specialist | 3 | UX Design Agent | Sob demanda | medium |
| 17 | Software Architect | Specialist | 1 | Product & Engineering Director | Sob demanda | critical |
| 18 | Tech Lead Agent | Core | 2 | Product & Engineering Director | Diário | high |
| 19 | Frontend Senior Dev | Specialist | 3 | Tech Lead Agent | Sob demanda | high |
| 20 | Frontend Mid Dev | Specialist | 4 | Tech Lead Agent | Sob demanda | medium |
| 21 | Frontend Junior Dev | Specialist | 5 | Tech Lead Agent | Sob demanda | low |
| 22 | Backend Senior Dev | Specialist | 3 | Tech Lead Agent | Sob demanda | high |
| 23 | Backend Mid Dev | Specialist | 4 | Tech Lead Agent | Sob demanda | medium |
| 24 | Backend Junior Dev | Specialist | 5 | Tech Lead Agent | Sob demanda | low |
| 25 | Integration Agent | Specialist | 3 | Tech Lead Agent | Sob demanda | medium |
| 26 | QA Agent | Specialist | 3 | Tech Lead Agent | Por release | medium |
| 27 | DevOps Agent | Core | 2 | Tech Lead Agent | Diário | high |
| 28 | Database Architect | Specialist | 3 | Tech Lead Agent | Sob demanda | medium |
| 29 | Tech Writer Agent | Specialist | 5 | Tech Lead Agent | Por release | low |
| 30 | Security Architect | Specialist | 1 | Product & Engineering Director | Sob demanda | critical |
| 31 | AppSec Agent | Specialist | 3 | Security Architect | Por release | medium |
| 32 | Vulnerability Agent | Reactive | 6 | Security Architect | Semanal | medium |
| 33 | Compliance Security Agent | Specialist | 3 | Security Architect | Trimestral | medium |
| 34 | Revenue Director | Core | 2 | CEO | Semanal | critical |
| 35 | Growth Agent | Core | 6 | Revenue Director | Diário | medium |
| 36 | SEO Agent | Reactive | 5 | Growth Agent | Semanal | low |
| 37 | Content Agent | Core | 3 | Growth Agent | Diário | medium |
| 38 | Community Agent | Core | 3 | Growth Agent | Diário | medium |
| 39 | Demand Gen Agent | Specialist | 2 | Growth Agent | Semanal | high |
| 40 | Sales Agent | Specialist | 2 | Revenue Director | Sob demanda | high |
| 41 | SDR Agent | Core | 3 | Sales Agent | Diário | medium |
| 42 | RevOps Agent | Specialist | 6 | Sales Agent | Semanal | medium |
| 43 | Partnership Agent | Specialist | 3 | Sales Agent | Quinzenal | medium |
| 44 | Customer Success Agent | Core | 2 | Revenue Director | Diário | high |
| 45 | Support Agent | Reactive | 5 | Customer Success Agent | Contínuo | medium |
| 46 | L2 Agent | Specialist | 3 | Customer Success Agent | Sob demanda | medium |
| 47 | Churn Prevention Agent | Specialist | 6 | Customer Success Agent | Semanal | medium |
| 48 | Expansion Agent | Specialist | 3 | Customer Success Agent | Mensal | medium |
| 49 | Finance & Compliance Director | Core | 2 | CEO | Semanal | critical |
| 50 | Finance Agent | Specialist | 6 | Finance & Compliance Director | Semanal | medium |
| 51 | Metrics Agent | Specialist | 6 | Finance & Compliance Director | Semanal | medium |
| 52 | Forecast Agent | Specialist | 6 | Finance & Compliance Director | Mensal | medium |
| 53 | Legal Agent | Specialist | 2 | Finance & Compliance Director | Sob demanda | high |
| 54 | Governance & Compliance Agent | Specialist | 2 | Finance & Compliance Director | Trimestral | high |
| 55 | Data Governance Agent | Specialist | 3 | Finance & Compliance Director | Mensal | medium |
| 56 | Data Lead Agent | Core | 2 | Finance & Compliance Director | Mensal | high |
| 57 | Data Engineer Agent | Specialist | 4 | Data Lead Agent | Sob demanda | medium |
| 58 | BI Agent | Core | 6 | Data Lead Agent | Semanal | medium |
| 59 | Data Science Agent | Specialist | 6 | Data Lead Agent | Sob demanda | medium |

## Fontes

- Documento de origem: `Arquitetura de Agentes — Micro-empresa.md` (V6)
- Especificação: [agentcompanies.io/specification](https://agentcompanies.io/specification)
- Runtime: [Paperclip](https://github.com/paperclipai/paperclip)
- Skills: [SKILLS_AI](https://github.com/TechMinds-Group/SKILLS_AI)

## Getting Started

```
npx paperclipai company import --from ./AGENTS_IA
```
