# Repository agent instructions

This repository uses [architecture decision records](docs/adrs/README.md) for durable architecture choices. Before changing architecture, source ownership, public contracts, security boundaries, migrations, delivery, or validation policy, read the index and the applicable ADR Short and Long variants. The Long variant is canonical; Guides explain mechanics.

Only **Accepted** ADRs are binding. Proposed ADRs are pending maintainer decisions. Follow an Accepted successor when an ADR is Superseded. If a request conflicts with an Accepted ADR, name the decision and affected scope, then stop that part of the change until the maintainer accepts a successor or changes the request. Do not rewrite accepted history to match current code.

The [provider mapping](docs/architecture/provider-mapping.md) records Architecture Compass provenance and deferred candidates. It does not give provider decisions authority over this repository. Record validation evidence in [docs/architecture/receipts/](docs/architecture/receipts/); distinguish source inspection, local checks, CI, publication, deployment, and external proof. Name materially applied ADRs and unverified stages in final reports.

Keep changes within the user's authorized scope. Do not infer permission for publication, deployment, production access, destructive work, or global configuration changes from an ADR.
