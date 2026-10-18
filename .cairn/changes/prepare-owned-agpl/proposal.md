## Why

The operator authorizes AGPL-3.0-or-later for all new owned source, including reusable cores and contracts. This source preparation replaces the earlier permissive default prospectively without revoking prior grants.

## What Changes

- Align owned manifests, package-local grants, license-policy.tsv, notices, and existing documentation under AGPL-3.0-or-later.
- Cover owned schemas, fixtures, templates, examples, policy, and documentation.
- Preserve historical grants, imported code, exact dependency sources, canonical bytes, and receipts.

## Impact

- **Files**: Cargo manifests, owned license texts, license-policy.tsv, docs/licensing.md, README, and licensing requirements.
- **Testing**: Parent runs license-boundary positive/negative controls, Cargo metadata/package inspection, lifecycle gates, and unchanged projection freshness after implementation. No publication, runtime/API/format changes, dependency pin updates, or remote actions.
