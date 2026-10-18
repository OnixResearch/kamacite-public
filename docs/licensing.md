# Kamacite licensing boundary

New owned modifications use AGPL-3.0-or-later. This is prospective source preparation, not publication.

| Surface | Current owned-source grant |
|---|---|
| `crates/kamacite-core/**`, `crates/kamacite-cli/**`, and `pilots/schema-migration/**` owned implementation | `AGPL-3.0-or-later` |
| Owned canonical schemas, reusable interchange fixtures, contracts, policy, configuration, templates, and generated projections | `AGPL-3.0-or-later` for new owned modifications |
| Owned repository documentation, tooling, and lifecycle material | `AGPL-3.0-or-later` for new owned modifications |
| Dependencies, immutable imports, upstream material in generated artifacts, and external references | Their recorded upstream grants, notices, and source identities |

The core must not depend on `kamacite-cli`. The CLI may depend on the core. Core consumers receive no implicit filesystem, evaluator, process, or network authority. Licensing does not change this architectural boundary or license independently authored user inputs merely because Kamacite processes them.

Complete current terms are in `LICENSE` and `LICENSES/AGPL-3.0-or-later.txt`; every owned package, including the standalone pilot, carries its local `LICENSE`. Historical MIT and Apache texts remain in `LICENSES` and the core's `LICENSE-MIT`/`LICENSE-APACHE` solely for previously covered grants and attribution, not as offers for new modifications. Copyright (c) Kamacite contributors.

Prior grants cannot be revoked. Byte-identical previously covered content retains its earlier choices even in a current checkout. New owned modifications do not acquire a new MIT/Apache grant. Locked dependency sources and third-party material keep their original terms; no consumer pin is moved and no immutable fixture, proof/codec baseline, historical lifecycle archive, or receipt is rewritten.

Package licensing is outside canonical envelope, Preserves-value, adapter, target-artifact, and receipt identity unless a versioned schema explicitly includes it. This preparation does not change canonical bytes, formats, Rust APIs, or runtime semantics. This map does not establish legal compliance or behavioral correctness.
