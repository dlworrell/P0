# Atarix Documentation Inventory Addendum 001

Status: Preliminary enumeration addendum

Parent issue: P0 #1
Related sub-issue: P0 #7
Target repository: `dlworrell/atarix`

## Purpose

This addendum records additional documentation artifacts discovered after the initial Atarix documentation inventory was created.

It does not move, merge, delete, or rewrite Atarix files.

## Method

The current environment cannot perform a direct full `git clone` of GitHub. Enumeration therefore proceeds through the GitHub connector and repository search results.

Because this is not yet a true full-tree walk, these results are still preliminary. They should be merged into the primary inventory only after P0 #7 confirms complete enumeration.

## Newly Discovered Documentation Artifacts

| Current path | Artifact type | Provisional category | Status | Notes |
|---|---|---|---|---|
| `docs/design-rationale-history-v1.md` | rationale/history | reference/research | known | Design-rationale history document discovered during README/documentation search. |
| `docs/cpu-test-suite-integration-v1.md` | testing/integration | verification/process | known | CPU test-suite integration document discovered during README/documentation search. |
| `docs/resource-type-registry-v1.md` | registry | specification/reference | known | Resource type registry; should be considered alongside service and operation registries. |
| `docs/capability-record-format-v1.md` | specification | specification | known | Capability record format; likely related to capability model and ATX-SPEC-003. |

## Enumeration Notes

Additional searches confirmed or reinforced the presence of:

- `docs/service-id-registry-v1.md`
- `docs/service-directory-format-v1.md`
- `docs/operation-id-registry-v1.md`
- `docs/identity-eeprom-v1.md`
- `docs/card-health-model-v1.md`
- `docs/adr/ADR-00X-capability-evaluation-model.md`
- `docs/ADR-RING-SECURITY-MODEL.md`
- `docs/ADR-IDENTITY-TRUST-CAPABILITY-SEPARATION.md`
- `docs/ADR-THREE-FABRIC-ARCHITECTURE.md`

These entries were already present in the initial inventory or related findings, but should be rechecked during the metadata pass.

## Open Enumeration Questions

1. `ATX-SPEC-001`, `ATX-SPEC-012`, and `ATX-SPEC-017` were not confirmed as standalone files in this pass.
2. ATX-100 chapter enumeration remains incomplete.
3. Repository search is not a substitute for a real full-tree walk.
4. Generated files and support scripts still need explicit inclusion/exclusion decisions under P0 #6.

## Next Action

Continue P0 #7 by finding a reliable full-tree listing method through the GitHub connector or by using a local clone outside this restricted environment.
