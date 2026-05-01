# WHITE PAPER - TWINS PRODUCTION AI / ORA ECOSYSTEM

Version 1.1 - Avril 2026
Repository: `TwinsProductionAI/TwinsProductionAI`
Status: public ecosystem white paper

## Resume executif

TwinsProductionAI publie un ensemble de depots autour d'ORA Core OS. L'objectif est de structurer une approche modulaire pour assistants LLM: architecture, runtime, retrieval, specifications, langage, regulation et console produit.

La version 1.1 clarifie la carte d'ensemble, le role de chaque depot, la frontiere public/prive et la roadmap de stabilisation. L'ecosysteme ne doit pas etre lu comme une simple collection de prompts, mais comme une tentative de separer les responsabilites d'un systeme LLM gouverne.

## 1. Probleme vise

Les projets LLM deviennent difficiles a maintenir lorsque les prompts, les sources, les modules, les tests et les interfaces sont melanges.

Les symptomes les plus frequents sont:

- consignes trop longues et peu auditables;
- absence de separation entre architecture, runtime et produit;
- reponses fluides mais peu verifiees;
- documentation difficile a suivre;
- confusion entre donnees publiques et donnees client;
- couts inutiles lies aux boucles et au surtraitement;
- difficulte a expliquer le comportement du systeme.

L'ecosysteme ORA separe ces couches afin de faciliter la lecture, l'audit, l'evolution et l'adoption.

## 2. Vision

La vision de TwinsProductionAI est de rendre les systemes LLM plus structurables et plus gouvernables.

Cette vision repose sur quatre principes:

1. Une architecture doit etre lisible avant d'etre automatisee.
2. Les modules doivent avoir des responsabilites distinctes.
3. Les faits, les sources et les limites doivent etre traites explicitement.
4. L'adoption exige une interface simple pour les humains et des contrats stables pour les machines.

## 3. Carte des depots

### `ora-core-os`

Point d'entree principal. Il documente l'architecture, l'ordre canonique des modules, les guides d'installation et le white paper maitre.

### `ora-core-runtime`

Couche executable. Elle transforme les specifications en composants testables: parsing, registres, modules runtime, exemples et tests.

### `ora-core-rag`

Couche de retrieval gouvernee. Elle gere l'index local, les routes client, les traces d'audit et le RAG Governor.

### `ora-core-specs`

Depot documentaire technique. Il contient les specifications, white papers, schemas et notes d'integration.

### `grenaprompt-linked`

Couche de langage et de transport semantique. Elle documente GrenapromptLinked, GL, GPL et GL_G.

### `ora-core-neroflux`

Module de regulation de routage. Il aide a choisir une cadence, une route de traitement et des limites de fanout.

### `ora-core-legacy-whitepaper`

Archive historique. Elle garde les anciens documents pour la tracabilite du projet.

### `ora-companion-console`

Console produit. Elle vise l'adoption par plans, workspaces, connecteurs, logs et documentation d'usage.

## 4. Architecture globale

```text
User / Client
  -> ORA Companion Console
  -> ORA Core OS
  -> ORCHESTRATEUR_LLM
  -> GPV2 / GL / GL_G
  -> ORA Core RAG when source context is required
  -> Runtime modules
  -> Governance / verification modules when required
  -> Final bounded answer
  -> Audit trace
```

Cette architecture distribue les responsabilites. Le depot principal porte l'ordre et la structure. Le runtime execute. Le RAG recupere. Les specs documentent. La console rend l'ensemble utilisable.

## 5. Positionnement

L'ecosysteme se positionne comme une architecture de gouvernance LLM. Il ne se limite pas au prompt engineering.

Il documente des couches distinctes pour:

- structurer le comportement;
- transporter des etats semantiques;
- verifier ou borner les claims;
- recuperer des sources;
- separer les donnees client;
- produire des traces;
- fournir une interface d'adoption.

## 6. Frontiere public / prive

Public:

- architecture;
- specifications;
- white papers;
- exemples generiques;
- runtime public;
- schemas et manifests;
- documentation de recherche.

Prive:

- playbooks client;
- secrets;
- connecteurs sensibles;
- onboarding commercial;
- informations de tenants;
- documents operationnels specifiques;
- configurations de production.

Cette frontiere permet de publier le savoir technique sans exposer les donnees client ou la strategie commerciale sensible.

## 7. Mode d'adoption

L'adoption peut suivre trois niveaux:

### Lecture publique

Un lecteur consulte les white papers, specs et README pour comprendre la structure.

### Prototype local

Un developpeur utilise le runtime et le RAG pour tester localement des comportements.

### Plateforme accompagnee

Une equipe utilise ORA Companion Console pour gerer plans, workspaces, connecteurs, actions et logs.

## 8. Risques a surveiller

L'ecosysteme doit eviter:

- surcomplexite;
- multiplication de modules non testes;
- claims de performance non mesures;
- documentation redondante;
- confusion entre public et prive;
- interface trop technique pour le grand public;
- manque de tests de non-regression.

La meilleure defense est une combinaison de documentation claire, tests, exemples, et limites explicites.

## 9. Evaluation recommandee

Les prochaines evaluations devraient mesurer:

- coherence entre executions similaires;
- qualite des reponses source-backed;
- taux de claims bornes ou verifies;
- non-contamination entre routes client;
- cout en tokens;
- latence;
- comprehension par utilisateur non technique;
- facilite d'installation;
- lisibilite de l'audit.

Ces mesures doivent etre presentees comme contextuelles. Elles ne doivent pas devenir des promesses universelles.

## 10. Roadmap globale

1. Stabiliser les white papers principaux.
2. Relier tous les README aux documents correspondants.
3. Ajouter des tests publics de coherence.
4. Ajouter CI pour runtime et RAG.
5. Produire une demo locale end-to-end.
6. Renforcer ORA Companion Console.
7. Documenter l'Academy.
8. Preparer un pack PME pilote.
9. Clarifier licences, marques et conditions commerciales.
10. Publier des benchmarks reproductibles.

## Conclusion

L'ecosysteme ORA cherche a rendre les systemes LLM plus structurables, plus lisibles et plus auditables. Sa force vient de la separation des depots et de la clarification des responsabilites entre architecture, execution, retrieval, specifications, langage, regulation et interface produit.

La version 1.1 fixe une direction claire: moins de promesse abstraite, plus de couches nommees, de contrats, de documentation et de tests.
