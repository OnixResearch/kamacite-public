# Kamacite Owned Source Licensing

## MODIFIED Requirements

### Requirement: Package licensing follows the core-shell split

r[kamacite.packaging.license_boundary.package_split] All current and new Kamacite-owned packages, including kamacite-core, kamacite-cli, and owned pilots, MUST declare AGPL-3.0-or-later while preserving prior grants and third-party source terms.

#### Scenario: Package metadata is consumed

- GIVEN a consumer inspects current owned package metadata
- WHEN it chooses the core, CLI, or owned pilot
- THEN the package MUST offer AGPL-3.0-or-later without revoking older grants.

### Requirement: The split is validated in both directions

r[kamacite.packaging.license_boundary.validation] Focused validation MUST accept the owned AGPL mapping and MUST reject permissive declarations for current owned packages without changing pinned dependency licenses.

#### Scenario: Owned metadata becomes permissive accidentally

- GIVEN an owned package inherits or declares MIT OR Apache-2.0
- WHEN license-boundary validation runs
- THEN validation MUST fail with package-specific diagnostics.

### Requirement: Owned reuse surfaces use the selected grant

r[kamacite.packaging.license_boundary.owned_reuse] New Kamacite-owned canonical schemas, reusable fixtures, contracts, documentation, policy, and templates MUST be offered under AGPL-3.0-or-later without rewriting immutable canonical artifacts, imported source, or historical receipts.

#### Scenario: A recipient reuses a schema

- GIVEN a recipient inspects a new owned schema or fixture
- WHEN it consults the repository license map
- THEN the current grant MUST be explicit and historical byte-identical grants MUST remain effective.
