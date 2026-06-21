# CAN-005 – Engineering Glossary

Status: Draft

## Purpose

The Engineering Glossary defines project vocabulary used across AES, Project Zero, Catalyst, Atarix, and dependent repositories.

It exists to reduce ambiguity, preserve meaning, and help future contributors understand terms as the project uses them.

## Glossary Rule

A glossary term should define project meaning, not merely dictionary meaning.

If a word is used in an ordinary way, it does not need a glossary entry. If the project gives a word special engineering significance, it should be defined here.

## Entry Format

Each glossary entry should include:

- Term
- Definition
- Context
- Related documents, when known

## Initial Terms

### AES

The Atarix Engineering Standard.

AES is the canonical engineering record for the Catalyst and Atarix ecosystem. It contains engineering creed, standards, decision records, research notes, case studies, templates, and references.

Related: README, CAN-001

### Project Zero

The foundation phase for the Catalyst ecosystem.

Project Zero establishes the engineering constitution, lineage, glossary, mindset, documentation discipline, and traceability model before dependent implementation work accelerates.

Related: CAN-001, AES-100

### Catalyst

The broader ecosystem that inherits AES engineering governance.

Catalyst may include software, hardware, tools, documentation, repositories, and operating-system work that depend on AES standards and discipline.

Related: README, CAN-001

### Atarix

A dependent engineering project within the Catalyst ecosystem.

Atarix inherits AES engineering governance while retaining its own implementation-specific repository state, design records, and technical artifacts.

Related: README, CAN-001

### Canonical Engineering Record

The repository or document set treated as authoritative for engineering state.

For AES-level principles, process, and traceability, this repository is the canonical engineering record.

Related: README, CAN-001

### Provenance

The recorded origin of an idea, decision, document, requirement, or change.

Provenance helps future maintainers understand where something came from and why it exists.

Related: CAN-001, CAN-004

### Traceability

The ability to follow a requirement, decision, rationale, or change across documents, commits, issues, and implementation artifacts.

Traceability allows future contributors to reconstruct engineering reasoning instead of guessing intent from final artifacts alone.

Related: CAN-001

### Engineering Constitution

The foundational working rules that constrain how Project Zero and the broader ecosystem perform engineering work.

The constitution does not replace detailed standards. It constrains them.

Related: CAN-001

### Intellectual Lineage

The visible record of ideas, traditions, systems, and engineering cultures that influenced the project.

Lineage records influence. It does not grant unquestioned authority.

Related: CAN-004

### Observe, Understand, Improve

The first AES principle.

The current state must be observed before it is interpreted, and it must be understood before it is changed.

Related: README, CAN-001, AES-100

## Maintenance

This glossary should grow as project language stabilizes.

Do not overload it with speculative terminology. Add terms when they clarify committed work or prevent recurring ambiguity.
