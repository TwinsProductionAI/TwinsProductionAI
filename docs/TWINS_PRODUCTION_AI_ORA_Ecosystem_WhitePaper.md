# WHITE PAPER - TWINS PRODUCTION AI / ORA ECOSYSTEM

Version 1.0 - Avril 2026
Repository: `TwinsProductionAI/TwinsProductionAI`
Status: public ecosystem white paper

## Resume executif

TwinsProductionAI publie un ensemble de depots autour d'ORA Core OS. L'objectif est de structurer une approche modulaire pour assistants LLM: architecture, runtime, retrieval, specifications, langage, regulation et console produit.

## Carte des depots

- `ora-core-os`: architecture principale et ordre canonique des modules.
- `ora-core-runtime`: runtime executable, exemples et tests.
- `ora-core-rag`: retrieval local-first, routes, audit et RAG Governor.
- `ora-core-specs`: specifications techniques et white papers.
- `grenaprompt-linked`: langage et transport semantique GL, GPL et GL_G.
- `ora-core-neroflux`: regulation de routage et cadence de traitement.
- `ora-core-legacy-whitepaper`: archive historique.
- `ora-companion-console`: plateforme produit avec plans, connecteurs et logs.

## Probleme vise

Les projets LLM deviennent difficiles a maintenir lorsque les prompts, les sources, les modules, les tests et les interfaces sont melanges. L'ecosysteme ORA separe ces couches afin de faciliter la lecture, l'audit et l'evolution.

## Architecture globale

```text
User / Client
  -> ORA Companion Console
  -> ORA Core OS
  -> ORCHESTRATEUR_LLM
  -> GPV2 / GL / GL_G
  -> ORA Core RAG when source context is required
  -> Runtime modules
  -> Final bounded answer
  -> Audit trace
```

## Positionnement

L'ecosysteme se positionne comme une architecture de gouvernance LLM. Il ne se limite pas au prompt engineering. Il documente des couches distinctes pour structurer le comportement, verifier les sources, transporter les etats semantiques et rendre les integrations plus auditables.

## Frontiere public / prive

Public:

- architecture;
- specifications;
- white papers;
- exemples generiques;
- runtime public;
- schemas et manifests.

Prive:

- playbooks client;
- secrets;
- connecteurs sensibles;
- onboarding commercial;
- informations de tenants;
- documents operationnels specifiques.

## Roadmap

1. Stabiliser les white papers principaux.
2. Relier les README aux documents correspondants.
3. Ajouter des tests publics de coherence.
4. Ajouter CI pour runtime et RAG.
5. Produire une demo locale end-to-end.
6. Renforcer ORA Companion Console.
7. Documenter l'Academy.
8. Preparer un pack PME pilote.

## Conclusion

L'ecosysteme ORA cherche a rendre les systemes LLM plus structurables, plus lisibles et plus auditables. Sa force vient de la separation des depots et de la clarification des responsabilites entre architecture, execution, retrieval, specifications, langage et interface produit.
