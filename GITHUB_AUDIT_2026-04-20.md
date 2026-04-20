# TwinsProductionAI GitHub Audit - 2026-04-20

Scope: public repositories accessible through the TwinsProductionAI GitHub app.

Excluded from recommendations by owner request: TikTok, games, Nexus Arcana, Playdate/game SDK topics.

## Public Repository Order

1. `TwinsProductionAI/TwinsProductionAI` - public profile and visitor map.
2. `TwinsProductionAI/Coeur_ORA_GrenaPrompt_repo` - canonical ORA Core OS repository. Suggested future slug: `ora-core-os`.
3. `TwinsProductionAI/ora-core-runtime` - runtime package.
4. `TwinsProductionAI/ora-core-rag` - local retrieval, route gate and RAG governor.
5. `TwinsProductionAI/ora-core-specs` - schemas and public specs.
6. `TwinsProductionAI/grenapromptlinked-v1` - Grenaprompt Linked protocol. Suggested future slug: `grenaprompt-linked`.
7. `TwinsProductionAI/gpv2-exotique-neroflux` - Neroflux/Aletheia module package. Suggested future slug: `ora-core-neroflux`.
8. `TwinsProductionAI/Coeur-ORA-GrenaPrompt` - legacy whitepaper/archive. Suggested future slug: `ora-core-legacy-whitepaper` and archived status.

## Problems Fixed

- Public profile README now gives visitors a clear start map and repo order.
- Public READMEs were rewritten across the accessible repos to clarify roles and boundaries.
- `Coeur-ORA-GrenaPrompt` is now marked as legacy/archive material in its README.
- `gpv2-exotique-neroflux` no longer advertises a Python package without code on `main`; package files, schemas, examples and tests were added.
- `ora-core-rag` now has the ARCH+ activation runtime on `main`: CLI command, module, docs, schema, example, spec and tests.
- `Coeur_ORA_GrenaPrompt_repo` now has ARCH+ v3 as an M10 variant on `main`: docs, module spec, manifest entry, module index and declarative tests.
- Divergent PRs that had been manually integrated were closed to avoid stale public work.
- `ora-core-specs/PUBLISH_TO_GITHUB.md` was changed from an obsolete publication checklist into a current publication status note.
- `Coeur-ORA-GrenaPrompt/docs/ORA_CORE LIGHT DEMO` was rewritten as a legacy archive note and no longer claims active runtime guarantees such as a 24h learning loop or a fixed error margin.

## Verification

- Accessible repositories found: 8.
- Visibility: all 8 accessible repositories are public.
- Open PRs after cleanup: none found in the accessible repos.
- Local unpublished repo check: only `C:\gpv2-exotique-neroflux` and `C:\ora-core-rag` appeared as local Git work folders; both point to public TwinsProductionAI repositories.
- Local tests passed:
  - `gpv2-exotique-neroflux`: 9 tests passed.
  - `ora-core-rag`: 26 tests passed.
- Search exclusions:
  - `TikTok`: no accessible code-search result.
  - `Nexus Arcana`: no accessible code-search result.
  - `game`: no accessible code-search result.
  - `jeu`: only French-language spec hits, not game projects.

## Remaining Blockers

The current GitHub app tools can edit repository contents and PR state, but they do not expose repository metadata operations. These items still require GitHub UI, `gh`, or an authenticated repository settings API:

- Rename `Coeur_ORA_GrenaPrompt_repo` to `ora-core-os`.
- Rename `grenapromptlinked-v1` to `grenaprompt-linked`.
- Rename `gpv2-exotique-neroflux` to `ora-core-neroflux`.
- Rename or archive `Coeur-ORA-GrenaPrompt` as `ora-core-legacy-whitepaper`.
- Pin the recommended repos in profile order.
- Update repository descriptions and topics.

## Recommended Naming Rule

Use lowercase kebab-case for public repository slugs:

- `ora-core-*` for ORA system components.
- `grenaprompt-*` for protocol/language artifacts.
- `*-legacy-*` for historical archives.
- Avoid mixed separators, accents, spaces and vague suffixes like `_repo` or `v1` unless the version is the actual product identity.
