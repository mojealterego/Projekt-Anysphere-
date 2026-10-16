# Roadmapa Projekt Anysphere

Statusy: [ ] planowane; [x] zrealizowane i zweryfikowane. Etapy realizować po spełnieniu kryteriów odbioru, nie wyłącznie na podstawie deklaracji.

## Fundamenty
- [x] P-000: Utworzenie podstawowego opisu, architektury i rejestru ryzyk w repozytorium.
- [ ] P-001: Monorepo, workspace Rust/TypeScript, lint, format, unit tests i CI.
- [ ] P-002: Kontrakty API, model domenowy, versioning i schema migrations.
- [ ] P-003: IAM, RBAC/ABAC, tenant isolation, audyt operacji i secrets management.
- [ ] P-004: Telemetria OpenTelemetry, metryki, tracing, logi i SLO.

## Analiza kodu i kontekst
- [ ] P-010: Ingestion repozytoriów, ignore rules, kontrola uprawnień i incremental indexing.
- [ ] P-011: Parser Tree-sitter i ekstrakcja symboli.
- [ ] P-012: Integracja LSP i rozwiązywanie referencji między plikami.
- [ ] P-013: Graf zależności i zapytania z provenance.
- [ ] P-014: Hybrydowe retrieval: grep/ripgrep, AST, graf i opcjonalne embeddings.
- [ ] P-015: Context packing, deduplikacja i ocena trafności.

## Runtime agentów
- [ ] P-020: Orchestrator, planner, executor, verifier i policy engine.
- [ ] P-021: Trwały state graph, checkpointy, recovery, idempotencja.
- [ ] P-022: Model routing, BYOK, limity kosztów i budżety tokenów.
- [ ] P-023: MCP tool gateway, allowlist, timeouts i audyt.
- [ ] P-024: Git worktree isolation i bezpieczne scalanie zmian.
- [ ] P-025: Sandboxed execution (kontenery/microVM), kontrola sieci i zasobów.
- [ ] P-026: Współbieżność, scheduler, kolejki, backpressure i cancellation.
- [ ] P-027: Autonomiczne zadania w tle z zatwierdzaniem działań wysokiego ryzyka.

## Środowisko i interfejsy
- [ ] P-030: CLI i lokalny daemon.
- [ ] P-031: Web IDE i edytor kodu.
- [ ] P-032: Cloud Agent Builder — Code i NoCode.
- [ ] P-033: Desktop Agent Builder — Windows/macOS, Code i NoCode.
- [ ] P-034: Mobile Agent Builder — Android/iOS, Code i NoCode.
- [ ] P-035: Wizualizacja planów, diffów, śladów i historii decyzji.

## Jakość, bezpieczeństwo i wydania
- [ ] P-040: Integracja GitHub PR, webhook verification i CI/CD.
- [ ] P-041: Agent code review, SAST, SCA, secret scanning i quality gates.
- [ ] P-042: Pętle naprawcze z limitem iteracji, rollback i eskalacją.
- [ ] P-043: Testy unit, integration, contract, e2e i property-based.
- [ ] P-044: Red team prompt injection, SSRF, path traversal i supply chain.
- [ ] P-045: Testy wielotenantowe, chaos engineering i disaster recovery.
- [ ] P-046: Niezależny audyt, akceptacja operatora i release gates.

## Produkt i finansowanie
- [ ] P-050: Walidacja problemu, segmentów klientów i konkurencji.
- [ ] P-051: Model kosztów inference, compute, storage i wsparcia.
- [ ] P-052: Plan MVP, KPI, pilotaż i mierzalne kryteria product-market fit.
- [ ] P-053: Korekta wniosku dotacyjnego i weryfikacja źródeł oraz prognoz.

## Zasada aktualizacji
Po każdej zmianie kodu aktualizować stan odpowiednich etapów, dowody testowe, datę i odnośnik do commitów. Nie oznaczać zadań jako ukończonych bez dowodów.
