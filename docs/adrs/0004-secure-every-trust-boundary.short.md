# ADR-0004: Secure every trust boundary

ID: ADR-0004
Title: Secure every trust boundary
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: security-data
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Short

Variants: [Short](0004-secure-every-trust-boundary.short.md) · [Long, canonical](0004-secure-every-trust-boundary.long.md) · [Guide](0004-secure-every-trust-boundary.guide.md)

## Decision summary

At each identity, data, privilege, code, or system boundary, validate input and output, authenticate and authorize where relevant, minimize sensitive data, and grant least privilege. Fail closed when a control is unknown.

This proposal is pending maintainer acceptance; it does not authorize implementation.
