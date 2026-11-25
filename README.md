# TwinsProductionAI

Public workspace for ORA Core OS, GrenapromptLinked, and verifiable LLM governance.

ORA Core is a modular AI architecture built around factual governance, semantic transport, deterministic runtime layers, and auditable retrieval.

## ORA Core Hub — official platform / plateforme officielle

**Twins Productions IA** (GitHub: TwinsProductionAI) develops the ORA ecosystem.

- **ORA Core OS** — modular architecture and governance specifications for existing language models.
- **ORA Core Hub** — training and tools for structured instructions, reusable AI workflows and governance. Official platform: [oracorehub.com](https://oracorehub.com/).
- **ORA Knowledge Gateway** — public, read-only documentation and evidence resources, accessible without an account or JavaScript: [knowledge.oracorehub.com](https://knowledge.oracorehub.com/).
  - [Full public corpus / Connaissance](https://knowledge.oracorehub.com/connaissance/)
  - [Machine-readable resource index](https://knowledge.oracorehub.com/llms.txt)
  - [Evidence registry (JSON)](https://knowledge.oracorehub.com/connaissance/evidence.json)
  - [Public GitHub mirror](https://github.com/TwinsProductionAI/ora-core-os/tree/main/knowledge)

The public documentation distinguishes published specifications, internal qualifications, reported user experiences and independently validated performance. Publication alone does not establish performance gains. Private and premium resources remain outside this public corpus.

## ORA Open Lab — Machine First

Public experimental protocol v0.3.0 for comparing four prompt conditions on two fictitious tasks (eight prompts). No comparative results have been published. Execution requires isolated sessions or an external orchestrator; reading the protocol is not an experiment.

- [Open Lab — public experimental documentation](https://knowledge.oracorehub.com/open-lab/)
- [Machine-readable protocol JSON](https://knowledge.oracorehub.com/open-lab/protocol.json)
- [Manifest and SHA-256](https://knowledge.oracorehub.com/open-lab/manifest.json)
- [Independent review and result receipt schema](https://knowledge.oracorehub.com/open-lab/receipt.schema.json)
- [Alternative Render origin](https://ora-knowledge-gateway.onrender.com/open-lab/)
- [Public implementation, fixtures and protocol generator (release commit)](https://github.com/TwinsProductionAI/ora-core-os/blob/04f2ea29ad7742c10b4892bf537a7cc430b6a284/knowledge/open-lab.cjs)
- [External HTTP and build validation](https://github.com/TwinsProductionAI/ora-core-os/actions/runs/45518612882)

Availability over HTTPS does not guarantee discovery, indexing, or retrieval by every LLM product. A failed retrieval in one environment is not evidence of global unavailability.

## Public Repository Map

| Layer | Repository | Public role |
| --- | --- | --- |
| Entry point | [ora-core-os](https://github.com/TwinsProductionAI/ora-core-os) | Public ORA Core OS architecture, GPV2 module map, installation order, and canonical documentation. |
| Technical specifications | [ora-core-specs](https://github.com/TwinsProductionAI/ora-core-specs) | Public specs, primitive registries, technical contracts, and short reference indexes. |
| Runnable runtime | [ora-core-runtime](https://github.com/TwinsProductionAI/ora-core-runtime) | Public runtime bundle for GPV2 parsing, GL/GL_G primitives, governance modules, samples, and tests. |
| Retrieval layer | [ora-core-rag](https://github.com/TwinsProductionAI/ora-core-rag) | Local-first retrieval, canon indexing, audit traces, route gates, and RAG governance. |
| Protocol language | [grenaprompt-linked](https://github.com/TwinsProductionAI/grenaprompt-linked) | GrenapromptLinked, GL, GPL, GL_G language notes, glossaries, and semantic transport references. |
| Multi-LLM install center | [ora-core-os-multi-llm](https://github.com/TwinsProductionAI/ora-core-os-multi-llm) | Deterministic multi-LLM install center and module catalog. |
| Flow control | [ora-core-neroflux](https://github.com/TwinsProductionAI/ora-core-neroflux) | Cognitive flow-control module and routing specification. |
| Historical archive | [ora-core-legacy-whitepaper](https://github.com/TwinsProductionAI/ora-core-legacy-whitepaper) | Historical ORA Core archive for earlier GL-CORE-LOCK white papers and audit references. |

## Public Scope

Public repositories contain:

- architecture and module maps
- technical canon and primitive registries
- public specifications and contracts
- runnable examples and validation tests
- short indexes and reference notes
- historical white paper archives

## Non-Public Scope

The following material is outside the public repository scope:

- full training courses
- exercises and quiz material
- certification content
- instructor notes
- commercial onboarding material
- client-specific delivery packs
- private operational notes

## Core Reading Order

1. [ora-core-os](https://github.com/TwinsProductionAI/ora-core-os)
2. [ora-core-specs](https://github.com/TwinsProductionAI/ora-core-specs)
3. [ora-core-runtime](https://github.com/TwinsProductionAI/ora-core-runtime)
4. [ora-core-rag](https://github.com/TwinsProductionAI/ora-core-rag)
5. [grenaprompt-linked](https://github.com/TwinsProductionAI/grenaprompt-linked)

## Positioning

This workspace publishes modules, verification contracts, governance layers, specifications, and runnable prototypes for auditable AI systems.