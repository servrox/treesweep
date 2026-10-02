# Architecture Compass provider mapping

This is provenance and a candidate review, not local architectural authority. The local ADR Long variants become binding only after explicit maintainer acceptance.

- Source: Architecture Compass 0.10.1, `references/adr-catalog.md`, SHA-256 `56e4732eac9398e9eb571fa40cabc41faf5ef34bdacddecfe532d0a053c438bd`
- Repository evidence: initial README only; no code, stack, deployable, tests, or CI.
- Coverage: `setup/recommended`. Seven foundation candidates are adapted as local Proposed ADRs. The remaining candidates are deferred until their trigger occurs.
- Eligible accepted target-repository provider candidates: 46. Selected: 7; deferred: 39; rejected: 0.
- Deferred owner: treesweep maintainers. Re-evaluate each candidate before the first change matching its trigger; a deferred provider decision has no local force.

| Provider | Candidate | Disposition | Local ADR | Trigger / evidence |
| --- | --- | --- | --- | --- |
| AC-ADR-005 | Make Repository ADRs Binding Agent Guardrails | Adapt as Proposed | [ADR-0001](../adrs/0001-govern-architecture-through-accepted-adrs.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-006 | Assign Workspace Ownership and Source Roles | Adapt as Proposed | [ADR-0002](../adrs/0002-assign-source-ownership-and-file-roles.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-007 | Enforce Runtime-Safe Module and Public Package Boundaries | Defer | — | Code crosses browser, trusted server, backend process, app, or package boundaries, or exposes a reusable package API. Owner: maintainers. |
| AC-ADR-008 | Compose Next.js Routes, Rendering, and Component Responsibilities | Defer | — | A Next.js App Router route, layout, fallback, screen, or interactive component boundary is created or materially changed. Owner: maintainers. |
| AC-ADR-009 | Choose Read, Query, Caching, and Freshness Boundaries | Defer | — | Data is read by Server Components, browser clients, external clients, or realtime consumers. Owner: maintainers. |
| AC-ADR-010 | Protect Writes Behind Validated Command Boundaries | Defer | — | Browser interaction, webhook, external client, or integration mutates trusted state. Owner: maintainers. |
| AC-ADR-011 | Compose Long-Running Backend Runtimes and Lifecycles Explicitly | Defer | — | Creating or refactoring a worker, service, HTTP process, route plugin, service registry, or dependency-injection boundary. Owner: maintainers. |
| AC-ADR-012 | Resolve Environment and Configuration at Deployable Boundaries | Defer | — | A deployable app reads environment variables, secrets, ports, URLs, feature configuration, or runtime configuration. Owner: maintainers. |
| AC-ADR-013 | Own Language, Package, Build, Lint, and Supply-Chain Tooling Explicitly | Defer | — | Establishing or changing a JavaScript/TypeScript compiler, package manager, workspace, task orchestration, lint/format toolchain, or dependency trust policy. Owner: maintainers. |
| AC-ADR-014 | Select Application Runtimes, Deployment Hosts, and Additional Targets by Evidence | Defer | — | Choosing or changing Next.js, Bun or Node.js, an HTTP framework, deployment hosting, mobile delivery, or desktop delivery. Owner: maintainers. |
| AC-ADR-015 | Select Frontend Capability Libraries by Product Need | Defer | — | Choosing validation, date/time, form, URL-state, internationalization, UI, styling, table, animation, chart, or email-rendering capabilities. Owner: maintainers. |
| AC-ADR-016 | Select AI Model, Streaming, UI, and Agent Capabilities Deliberately | Defer | — | A product adds model access, streamed generation, tool calls, AI-rendered UI, or agent orchestration. Owner: maintainers. |
| AC-ADR-017 | Select Relational, Cache, Queue, and Realtime Capabilities by Data Requirements | Defer | — | Choosing persistence, an ORM, cache, queue, rate limiting, or realtime transport. Owner: maintainers. |
| AC-ADR-018 | Validate Behavior at the Owning Boundary and Promote Enforcement Gradually | Adapt as Proposed | [ADR-0003](../adrs/0003-validate-behavior-at-the-owning-boundary.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-019 | Apply Security and Privacy Controls at Every Trust Boundary | Adapt as Proposed | [ADR-0004](../adrs/0004-secure-every-trust-boundary.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-020 | Define Data Ownership, Tenancy, Retention, and Deletion Before Access Paths | Defer | — | Introducing or changing persisted personal, tenant, device, generated, derived, or externally synchronized data. Owner: maintainers. |
| AC-ADR-021 | Preserve Compatibility Through Explicit Migrations and Deprecation Windows | Adapt as Proposed | [ADR-0005](../adrs/0005-migrate-contracts-explicitly.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-022 | Deliver Reversible Slices With Explicit Rollback and Promotion Gates | Adapt as Proposed | [ADR-0006](../adrs/0006-deliver-reversible-slices-with-promotion-gates.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-023 | Operate Services With Observable Health, Readiness, Failure, and Cleanup | Defer | — | A deployable runtime, job, queue, subscription, integration, or critical dependency is introduced or changed. Owner: maintainers. |
| AC-ADR-024 | Meet an Explicit Accessibility Baseline With Automated and Manual Proof | Defer | — | Building or changing user-facing content, navigation, forms, media, status, or interaction. Owner: maintainers. |
| AC-ADR-025 | Set Measurable Performance Budgets and Optimize From Evidence | Defer | — | A change affects rendering, bundles, network, cache, database, background work, resource use, or user-perceived latency. Owner: maintainers. |
| AC-ADR-027 | Use the Open Agent Skills Specification | Defer | — | Creating, validating, or publishing a repository of public Agent Skills. Owner: maintainers. |
| AC-ADR-028 | Keep Candidates Outside the Promoted Public Catalog | Defer | — | Creating a skill candidate or deciding whether it belongs in the public install surface. Owner: maintainers. |
| AC-ADR-029 | Promote Skills Through an Evidence and Maintenance Gate | Defer | — | Evaluating whether a candidate skill is ready for the promoted public catalog. Owner: maintainers. |
| AC-ADR-030 | License Public Skill Repositories Under Apache-2.0 | Defer | — | Establishing the license for a new public skill repository or changing its distribution terms. Owner: maintainers. |
| AC-ADR-031 | Keep Skill Evaluation Evidence Outside the Runtime Payload | Defer | — | Adding skill eval cases, rubrics, transcripts, run evidence, or runtime self-test fixtures. Owner: maintainers. |
| AC-ADR-032 | Keep Maintainer-Local Helper State Out of Public Repositories | Defer | — | Installing or recording maintainer-local agent helpers, generated host links, or helper lock state. Owner: maintainers. |
| AC-ADR-033 | Choose Portable Dependency-Light Skill Helpers | Defer | — | Adding or replacing an executable helper inside a public skill package. Owner: maintainers. |
| AC-ADR-035 | Classify Skill Portability Before Choosing Host Variants | Defer | — | Naming, placing, splitting, or adding host metadata to a public skill capability. Owner: maintainers. |
| AC-ADR-037 | Preserve Target Contracts and Gate Gateway Extraction | Defer | — | Routing a skill across execution hosts, splitting variants, or extracting a shared agent or model gateway. Owner: maintainers. |
| AC-ADR-038 | Gate Optional Capabilities and Tool Side Effects | Defer | — | A public skill can call an optional provider, install a missing tool, launch a browser, or use a higher-side-effect capability. Owner: maintainers. |
| AC-ADR-040 | Offer an Opinionated Stack Profile for New Public Skill Repositories | Defer | — | Architecture Compass sets up a new public skill repository and the user wants a concrete maintained starting stack. Owner: maintainers. |
| AC-ADR-041 | Publish Public Skills Through GitHub and the Open Skills CLI | Defer | — | Choosing or validating the public source, discovery, installation, and release path for a public skill repository. Owner: maintainers. |
| AC-ADR-049 | Distinguish Change Risk From Representative Environment Observation | Adapt as Proposed | [ADR-0007](../adrs/0007-classify-validation-risk-by-changed-contract.long.md) | New repository governance foundation; acceptance pending. |
| AC-ADR-054 | Isolate Agent Writes in External Git Worktrees | Defer | — | An agent may modify repository state, whether manually, through delegation, or through an orchestrator. Owner: maintainers. |
| AC-ADR-055 | Separate Change Impact From Generated Release Publication | Defer | — | A repository aggregates reviewed public-skill changes into generated release preparation and separately approved publication. Owner: maintainers. |
| AC-ADR-056 | Preserve Release Candidates Through Verified Protected History | Defer | — | A validated release waits for approval or retry after its protected branch advances. Owner: maintainers. |
| AC-ADR-057 | Separate Metadata Repair From Installable Artifact Provenance | Defer | — | A mutable published release is missing exact metadata or an installable artifact. Owner: maintainers. |
| AC-ADR-058 | Use pnpm for Package Management and Bun for Execution | Defer | — | Establishing or changing JavaScript/TypeScript package management, script execution, shell expressions, build tooling, tests, or server deployment artifacts. Owner: maintainers. |
| AC-ADR-059 | Own repository validation through discoverable framework tests | Defer | — | Adding or migrating repository-maintenance checks that assert configuration, source, documentation, generated-output or release contracts. Owner: maintainers. |
| AC-ADR-060 | Isolate test execution by effects and runtime contracts | Defer | — | Tests share mutable resources, spawn processes, access external systems or exercise runtime-specific behavior. Owner: maintainers. |
| AC-ADR-061 | Shard tests as complete fail-closed evidence sets | Defer | — | A required test obligation is distributed across workers, machines, platforms or independently reported jobs. Owner: maintainers. |
| AC-ADR-062 | Cache test transforms without reusing correctness | Defer | — | Persisting or restoring transformed test modules to reduce repeated validation work. Owner: maintainers. |
| AC-ADR-063 | Enforce Tailwind Design-System Contracts with shadcn lint | Defer | — | A Tailwind v4 repository adopts or changes mechanical enforcement of design-system usage in supported source files. Owner: maintainers. |
| AC-ADR-065 | Require Qualified Jev Host Advice after Repository Adoption | Defer | — | A repository elects to require qualified Jev capability advice through explicitly authorized agent hosts. Owner: maintainers. |
| AC-ADR-066 | Use Portless for Local Development Endpoints | Defer | — | Establishing, reviewing or changing local HTTP or WebSocket development endpoints, including single apps, monorepos and parallel worktrees. Owner: maintainers. |

## Scope notes

The repo does not yet publish a stable public skill with multiple material workflows; the conditional skill-selector instruction is **not applicable** on current evidence. Reassess if treesweep becomes such a repository.

No local Jev adoption decision exists. AC-ADR-065 is deferred until the maintainers explicitly choose to govern host capability advice for this repository; this mapping does not activate a hook, grant processing consent, or configure a host.
