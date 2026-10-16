# Architektura docelowa

Status: projekt koncepcyjny, nieimplementowany.

## Granice systemu
1. **Clients:** Web IDE, CLI, desktop i mobile builders.
2. **API Gateway:** authn/authz, rate limiting, tenant context.
3. **Control Plane:** orchestration, scheduler, state machine, policy engine, billing quotas.
4. **Intelligence Plane:** repo ingestion, Tree-sitter, LSP, dependency graph, hybrid retrieval, model router.
5. **Execution Plane:** isolated worktrees, ephemeral sandboxes, network egress policy, resource limits.
6. **Verification Plane:** tests, static analysis, review agents, PR workflows.
7. **Data Plane:** durable workflow state, encrypted secrets, audit logs, metadata, artifact store.

## Krytyczne kontrakty
- Każde narzędzie działa w kontekście tożsamości, tenanta i zakresu uprawnień.
- Nieufne dane z repozytorium i narzędzi nie mogą modyfikować polityki wykonania.
- Zapisy są audytowane, idempotentne lub zabezpieczone przed powtórzeniem.
- Agenty nie scalają ani nie wdrażają zmian bez odpowiedniego gate.
- Retry ograniczone budżetem, timeoutem i liczbą prób.
- Parser AST nie zastępuje semantycznej analizy LSP; graf zależności może być niekompletny.
- Retrieval jest hybrydowy, a nie dogmatycznie wyłącznie grafowy.

## Planowany stos
Rust (backend i runtime), TypeScript (UI), Tree-sitter, LSP, Git, OpenTelemetry, PostgreSQL, izolowane środowiska wykonawcze. Ostateczny wybór komponentów zależy od testów i ADR.
