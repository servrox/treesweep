# ADR-0007: Classify validation risk by changed contract

ID: ADR-0007
Title: Classify validation risk by changed contract
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: quality-delivery
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0007-classify-validation-risk-by-changed-contract.short.md) · [Long, canonical](0007-classify-validation-risk-by-changed-contract.long.md) · [Guide](0007-classify-validation-risk-by-changed-contract.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Low risk requires a localized, deterministic, reversible adjustment with one owner and no changed public, trust, data, infrastructure, or external-runtime contract. Behavioral changes beyond that are at least moderate; coupled or boundary-changing work requires stronger proof. Give each proof obligation one owner and a cadence: reuse, final-batch, checkpointed, or reproduce-first. Receipts include exact subject, candidate, command, toolchain, stage, environment, status, result, freshness, and invalidators. Run required gates before representative Preview proof. Production observation is only an already-authorized fallback for an exact, low-risk, reversible artifact and never replaces a gate.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
