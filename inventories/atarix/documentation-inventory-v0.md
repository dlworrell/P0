# Atarix Documentation Inventory v0

Status: Preliminary inventory

Parent issue: P0 #1
Sub-issues: P0 #6 through P0 #12
Target repository: `dlworrell/atarix`

## Purpose

This file begins the Project Zero documentation inventory for the Atarix operating-system repository.

The inventory is intentionally non-destructive. It records discovered documentation artifacts, provisional metadata, and follow-up work. It does not move, merge, delete, or rewrite any Atarix repository files.

## Inventory Scope

For this pass, a documentation artifact includes:

- Markdown documentation files
- repository README files
- architecture and specification documents
- ADRs and review records
- doctrine/process documents
- research notes
- documentation indexes or registries that affect documentation organization
- documentation-related CI notes

Source files, scripts, RTL files, and headers are not treated as documentation unless they are README-like, CI documentation, generated-document indexes, or explicit documentation support artifacts.

## Inventory Metadata Fields

| Field | Meaning |
|---|---|
| Current path | Path in `dlworrell/atarix` at time of discovery. |
| Artifact type | README, architecture, specification, ADR, review, doctrine, research, process, index, support, or unknown. |
| Provisional category | Proposed P0 category before migration. |
| Status | Known, draft, review-needed, duplicate-candidate, stale-candidate, or unknown. |
| Notes | Reasoning, uncertainty, relationship, or follow-up. |

## Directory Structure Observed So Far

```text
/
├── README.md
├── docs/
│   ├── *.md
│   ├── adr/
│   ├── architecture/
│   │   ├── ATX-100/
│   │   │   └── chapters/
│   ├── doctrine/
│   ├── engineering/
│   ├── research/
│   │   └── hashing/
│   └── reviews/
├── include/
│   └── atarix/
├── rtl/
│   └── atarix/
├── scripts/
│   ├── engineering/
│   └── rtl/
├── src/
└── tools/
    └── aems/
```

This structure is a first-pass documentation-related tree. It is not yet a complete repository tree.

## Discovered Documentation Artifacts

| Current path | Artifact type | Provisional category | Status | Notes |
|---|---|---|---|---|
| `README.md` | README | architecture/process | known | Root project description and architecture doctrine entry point. |
| `src/README.md` | README | process/reference | known | Source-tree README; needs content review. |
| `include/atarix/README.md` | README | specification/reference | known | Public include-tree README; needs content review. |
| `docs/security.md` | architecture | architecture | known | Security architecture or doctrine-adjacent document. |
| `docs/trust-model-v1.md` | architecture | architecture | known | Trust model. |
| `docs/capability-model.md` | architecture | architecture | known | Capability model; may overlap with ATX-SPEC-003. |
| `docs/bus-architecture.md` | architecture | architecture | known | Bus/fabric architecture candidate. |
| `docs/cpu-card-architecture-v1.md` | architecture | architecture | known | CPU-card architecture. |
| `docs/address-space-architecture.md` | architecture | architecture | known | Address-space architecture. |
| `docs/boot-sequence-v1.md` | architecture | architecture | known | Boot sequence. |
| `docs/interrupt-architecture-v1.md` | architecture | architecture | known | Interrupt architecture. |
| `docs/dma-engine-v1.md` | architecture | architecture | known | DMA engine. |
| `docs/supervisor-card-v1.md` | architecture | architecture | known | Supervisor card. |
| `docs/ulx3s-backplane-controller.md` | architecture | architecture | known | ULX3S/backplane controller. |
| `docs/rev-a-hardware-baseline.md` | architecture | reference/architecture | known | Hardware baseline. |
| `docs/timing-observability-v1.md` | architecture | architecture | known | Timing/observability. |
| `docs/cpu-observability-contract-v1.md` | specification | specification | known | CPU observability contract. |
| `docs/card-health-model-v1.md` | architecture/specification | architecture | known | Card health model. |
| `docs/card-identity-eeprom.md` | specification | specification | known | Card identity EEPROM; may overlap with identity-eeprom-v1. |
| `docs/identity-eeprom-v1.md` | specification | specification | known | Identity EEPROM v1; possible duplicate/iteration of card-identity-eeprom. |
| `docs/discovery-rom-format-v1.md` | specification | specification | known | Discovery ROM format. |
| `docs/service-directory-format-v1.md` | specification | specification | known | Service directory format. |
| `docs/service-id-registry-v1.md` | registry | specification/reference | known | Service ID registry. |
| `docs/operation-id-registry-v1.md` | registry | specification/reference | known | Operation ID registry. |
| `docs/netboot-ntp-v1.md` | architecture/specification | architecture | known | Netboot/NTP. |
| `docs/data-model-and-endianness.md` | specification | specification | known | Data model and endianness. |
| `docs/testing-strategy.md` | process | process | known | Testing strategy. |
| `docs/specification-roadmap.md` | roadmap | process | known | Specification roadmap. |
| `docs/gnu-dev-tools-setup.md` | process/toolchain | reference/process | known | Toolchain setup; may need modernization review. |
| `docs/vega816-analysis.md` | research | research | known | 65C816/VEGA816 research input. |
| `docs/fpga-instrumentation-testbench-services-v1.md` | specification | specification | known | FPGA instrumentation/testbench services. |
| `docs/ADR-RING-SECURITY-MODEL.md` | ADR | ADR | known | ADR outside `docs/adr/`; migration candidate. |
| `docs/ADR-DISCOVERABLE-OBSERVABLE-TESTABLE-INSTRUMENTABLE-RECOVERABLE.md` | ADR | ADR | known | ADR outside `docs/adr/`; migration candidate. |
| `docs/ADR-THREE-FABRIC-ARCHITECTURE.md` | ADR | ADR | known | ADR outside `docs/adr/`; migration candidate. |
| `docs/ADR-IDENTITY-TRUST-CAPABILITY-SEPARATION.md` | ADR | ADR | known | ADR outside `docs/adr/`; migration candidate. |
| `docs/adr/ADR-0014-testing-and-verification-strategy.md` | ADR | ADR | known | Numbered ADR. |
| `docs/adr/ADR-00X-capability-evaluation-model.md` | ADR | ADR | known | Placeholder-number ADR; needs numbering review. |
| `docs/doctrine/ARC-SEC.md` | doctrine | architecture/process | known | Security doctrine; root README references it. |
| `docs/doctrine/ARC-REVIEW.md` | doctrine/process | process | referenced | Referenced by root README; content not reviewed in this pass. |
| `docs/engineering/Documentation-Taxonomy-and-Style-Guide.md` | process | process | known | Documentation taxonomy/style. |
| `docs/engineering/Engineering-Gate.md` | process | process | known | Engineering gate. |
| `docs/reviews/architecture-review-template.md` | template | process | referenced | Referenced by root README; content not reviewed in this pass. |
| `docs/reviews/architecture-review-001.md` | review | review | known | Architecture review record. |
| `docs/reviews/Architecture-Review-002.md` | review | review | known | Architecture review record; filename case inconsistency. |
| `docs/reviews/Architecture-Review-003.md` | review | review | known | Architecture review record; filename case inconsistency. |
| `docs/reviews/ATX-SPEC-015-Reconciliation-Review.md` | review | review | known | Specification reconciliation review. |
| `docs/reviews/capability-sprint-1-review.md` | review | review | known | Capability sprint review. |
| `docs/research/hashing/krapivin-2025-open-addressing-summary.md` | research | research | known | Hashing research note. |
| `docs/architecture/architecture-backlog.md` | backlog | process/architecture | known | Architecture backlog. |
| `docs/architecture/ATX-100/index.md` | architecture index | architecture | known | ATX-100 architecture index. |
| `docs/architecture/ATX-100/chapters/01-purpose-and-scope.md` | architecture chapter | architecture | known | ATX-100 chapter. |
| `docs/architecture/ATX-100/chapters/15-lookup-acceleration.md` | architecture chapter | architecture | known | Lookup acceleration chapter. |
| `docs/architecture/ATX-100/chapters/20-aems-and-engineering-gates.md` | architecture chapter | architecture/process | known | AEMS/engineering gate chapter. |
| `docs/architecture/ATX-SPEC-002-Authority-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-003-Capability-Model.md` | specification | specification | known | ATX-SPEC series; may overlap with `docs/capability-model.md`. |
| `docs/architecture/ATX-SPEC-004-Lifecycle-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-005-Mailbox-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-006-Object-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-007-Namespace-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-008-Directory-Service-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-009-Resource-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-010-Audit-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-011-Error-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-013-Policy-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-014-Bootstrap-Security-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-015-POSIX-Compatibility-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-016-Supervisor-Management-Fabric.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-017-*` | specification | specification | referenced | Referenced by ATX-SPEC-021 dependency list, exact path not confirmed. |
| `docs/architecture/ATX-SPEC-018-Recovery-and-Reconciliation-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-019-Service-Model.md` | specification | specification | known | ATX-SPEC series. |
| `docs/architecture/ATX-SPEC-020-Hash-Table-and-Lookup-Acceleration-Model.md` | specification | specification | known | Lookup acceleration spec. |
| `docs/architecture/ATX-SPEC-020-Hardware-Mailbox-Integration-Notes.md` | integration note | architecture/research | known | Related to ATX-SPEC-020; possible supporting note. |
| `docs/architecture/ATX-SPEC-021-Memory-and-Data-Movement-Model.md` | specification | specification | indexed | Listed in `tools/aems/spec_index.json`. |
| `docs/architecture/ATX-SPEC-090-Atarix-Engineering-Management-System.md` | specification | specification/process | indexed | Listed in `tools/aems/spec_index.json`. |
| `docs/architecture/ATX-SPEC-091-Requirements-and-Traceability-Model.md` | specification | specification/process | indexed | Listed in `tools/aems/spec_index.json`. |
| `rtl/atarix/ATX-SPEC-020-CI.md` | CI documentation | process/verification | known | Documentation-like CI artifact outside docs tree. |
| `tools/aems/spec_index.json` | index | process/reference | known | AEMS spec index; not Markdown but documentation metadata. |

## Documentation Support Artifacts Observed

These are not primary documentation, but they affect documentation structure or validation.

| Current path | Artifact type | Provisional category | Status | Notes |
|---|---|---|---|---|
| `tools/check-doc-index.py` | support script | process/support | known | Documentation index checker. |
| `tools/check-md-links.py` | support script | process/support | known | Markdown link checker. |
| `tools/aems/build_docs_book.py` | support script | process/support | known | Documentation book builder. |
| `tools/aems/build_atx100.py` | support script | process/support | known | ATX-100 builder. |
| `tools/aems/migrate_docs_to_atx100.py` | support script | process/support | known | Migration support. |
| `tools/aems/aems.py` | support script | process/support | known | AEMS support script. |
| `scripts/engineering/run_gate.sh` | support script | process/support | known | Engineering gate runner. |
| `scripts/engineering/check_rtl_lint.sh` | support script | verification/support | known | RTL lint checker. |
| `scripts/rtl/run_atx_spec_020_sims.sh` | support script | verification/support | known | ATX-SPEC-020 simulation runner. |

## Immediate Findings

1. ADRs are split between `docs/` and `docs/adr/`.
2. Some filenames use inconsistent casing, especially under `docs/reviews/`.
3. `docs/capability-model.md` may overlap with `docs/architecture/ATX-SPEC-003-Capability-Model.md`.
4. `docs/card-identity-eeprom.md` may overlap with `docs/identity-eeprom-v1.md`.
5. `docs/architecture/ATX-SPEC-017-*` is referenced but not confirmed in this pass.
6. ATX-100 chapters are only partially enumerated in this pass.
7. Several documentation-support scripts exist and should be inventoried separately from project documentation.

## Next Actions

1. Confirm inventory scope under P0 #6.
2. Complete enumeration under P0 #7 using a reliable full-tree method if available.
3. Review content headings for each discovered document.
4. Fill in missing titles, statuses, and destination recommendations.
5. Do not move files until P0 #1 is closed and P0 #2 begins.
