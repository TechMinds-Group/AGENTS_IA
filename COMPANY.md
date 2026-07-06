---
name: Paperclip Micro-empresa SaaS B2B2C
description: Empresa de agentes autônomos operando um portfólio de produtos SaaS B2B2C. 59 agentes organizados em 4 blocos organizacionais (Governança & CEO, Produto & Engenharia, Revenue, Finanças & Compliance), coordenados via Paperclip e executados via OpenCode.
slug: paperclip-microempresa
schema: agentcompanies/v1
version: 6.0.0
license: MIT
authors:
  - name: TechMinds-Group
goals:
  - Hierarquia estrita de árvore: cada agente reporta a exatamente um superior
  - Responsabilidade atômica: escopo único e bem definido por agente para minimizar alucinação e desperdício de tokens
  - Toda task carrega product_id, product_summary, relevant_decisions e recovery_policy
  - Rollout gradual por confiança operacional, nunca em bloco
metadata:
  sources:
    - kind: github-repo
      repo: TechMinds-Group/SKILLS_AI
      usage: referenced
      attribution: TechMinds-Group
---

Paperclip Micro-empresa SaaS B2B2C é o pacote de agentes (Agent Companies / `agentcompanies/v1`) que implementa a Arquitetura de Agentes V6 do Paperclip-Organization: 59 agentes, 4 blocos organizacionais, 91 skills reutilizadas do catálogo [SKILLS_AI](https://github.com/TechMinds-Group/SKILLS_AI).

## Blocos organizacionais

| Bloco | Agentes | Líder |
|---|---|---|
| Governança & CEO | 6 | CEO |
| Produto & Engenharia | 27 | Product & Engineering Director |
| Revenue | 15 | Revenue Director |
| Finanças & Compliance | 11 | Finance & Compliance Director |

## Camada de execução

Todos os agentes rodam via adapter `opencode_local` (ver `.paperclip.yaml`). O modelo específico de cada agente (Tier/Modelo/Provider, ver `metadata` em cada `AGENTS.md`) é resolvido pela configuração do OpenCode, não fixado neste pacote.

## Fontes

- Documento de origem: `Arquitetura de Agentes — Micro-empresa.md` (V6, Paperclip-Organization)
- Especificação: [Agent Companies](https://agentcompanies.io/specification)
- Runtime: [Paperclip](https://github.com/paperclipai/paperclip)
- Skills: [SKILLS_AI](https://github.com/TechMinds-Group/SKILLS_AI)
