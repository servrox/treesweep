# Architecture decision records

The Long variant is canonical. **Proposed** decisions are pending maintainer acceptance and do not govern implementation. Accepted decisions bind future authorized architecture work. Accept a successor to change accepted intent; record both directions of the relationship.

## Proposed decisions

| ID | Decision | Status | Short | Long | Guide |
| --- | --- | --- | --- | --- | --- |
| ADR-0001 | Govern architecture through accepted ADRs | Proposed | [Short](0001-govern-architecture-through-accepted-adrs.short.md) | [Long](0001-govern-architecture-through-accepted-adrs.long.md) | [Guide](0001-govern-architecture-through-accepted-adrs.guide.md) |
| ADR-0002 | Assign source ownership and file roles | Proposed | [Short](0002-assign-source-ownership-and-file-roles.short.md) | [Long](0002-assign-source-ownership-and-file-roles.long.md) | [Guide](0002-assign-source-ownership-and-file-roles.guide.md) |
| ADR-0003 | Validate behavior at the owning boundary | Proposed | [Short](0003-validate-behavior-at-the-owning-boundary.short.md) | [Long](0003-validate-behavior-at-the-owning-boundary.long.md) | [Guide](0003-validate-behavior-at-the-owning-boundary.guide.md) |
| ADR-0004 | Secure every trust boundary | Proposed | [Short](0004-secure-every-trust-boundary.short.md) | [Long](0004-secure-every-trust-boundary.long.md) | [Guide](0004-secure-every-trust-boundary.guide.md) |
| ADR-0005 | Migrate contracts explicitly | Proposed | [Short](0005-migrate-contracts-explicitly.short.md) | [Long](0005-migrate-contracts-explicitly.long.md) | [Guide](0005-migrate-contracts-explicitly.guide.md) |
| ADR-0006 | Deliver reversible slices with promotion gates | Proposed | [Short](0006-deliver-reversible-slices-with-promotion-gates.short.md) | [Long](0006-deliver-reversible-slices-with-promotion-gates.long.md) | [Guide](0006-deliver-reversible-slices-with-promotion-gates.guide.md) |
| ADR-0007 | Classify validation risk by changed contract | Proposed | [Short](0007-classify-validation-risk-by-changed-contract.short.md) | [Long](0007-classify-validation-risk-by-changed-contract.long.md) | [Guide](0007-classify-validation-risk-by-changed-contract.guide.md) |

## Accepted decisions

None yet.

## Superseded and rejected decisions

None yet.

## Decision process

1. Propose one durable choice per ADR with an owner, status, scope, alternatives, consequences, and acceptance evidence.
2. The maintainer explicitly accepts, revises, or rejects the proposal. A proposed ADR alone never authorizes source changes.
3. For a changed accepted decision, add a successor with reciprocal `Supersedes` and `Superseded by` links. Preserve the prior accepted text.
4. Before architecture work, read the applicable Short and canonical Long variants. Use Guides only for mechanics and cite materially applied ADRs in the final report.
