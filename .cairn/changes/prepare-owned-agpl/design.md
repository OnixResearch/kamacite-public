## Context

Existing owned reusable surfaces offer MIT OR Apache-2.0 while the CLI offers AGPL. The operator explicitly selects AGPL-3.0-or-later for all new owned source.

## Decisions

### Decision: Prospective owned-source cutover

**Choice:** Change owned manifest defaults and local grants to AGPL-3.0-or-later; use the existing inventory checker and documentation map. Retain historical permissive texts as records, explicitly not grants for new modifications.

**Rationale:** One current owned-source declaration avoids a contradictory core/shell licensing promise while preserving irrevocable grants.

### Decision: Preserve immutable boundaries

**Choice:** Leave vendor imports, pinned source declarations, historical lifecycle archives/receipts, canonical fixture bytes, and third-party notices unchanged. State that licensing metadata is outside canonical identity and retain byte-identical prior grants.

**Rationale:** Ownership authorization does not rewrite history or third-party terms. This is source preparation, not distribution or publication.

## Risks / Trade-offs

- Byte-identical content already granted permissively remains available under that grant; new metadata cannot revoke it.
- Existing consumers on old Git pins retain old terms and are not migrated here.
- Parent verification is deferred; this active package must not be archived or represented as verified before evidence exists.
