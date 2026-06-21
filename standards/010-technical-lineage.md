# Technical Lineage

## Purpose

AEMS and Atarix are shaped by long-lived engineering projects that value portability, clarity, maintainability, security, and respect for users.

This document records the projects whose engineering practices influence the Just a Geek Engineering Standard. The goal is not to copy any one project wholesale, but to adopt proven habits deliberately.

## Primary Influences

### curl

curl demonstrates disciplined portable C engineering, careful API stability, security-conscious networking, and long-term maintainership.

Adopted principles:

- Portable C first.
- Stable public APIs.
- Clear separation between library and tool code.
- Conservative dependency choices.
- Security-sensitive review for network-facing code.
- Respect for existing users and platforms.

### Git

Git demonstrates portability, strong command-line discipline, careful compatibility decisions, and high-value commit messages.

Adopted principles:

- Live in the real world, not only in the paper standard.
- Avoid needless code churn.
- Make commit messages explain why, not only what.
- Match local style when modifying existing code.
- Prefer readable code over clever tricks.
- Document public APIs in the headers that expose them.

### SQLite

SQLite demonstrates small-core engineering, extreme reliability, public-domain-style accessibility, thorough testing, and careful stewardship of interfaces.

Adopted principles:

- Keep the core small and understandable.
- Treat tests as part of the product.
- Maintain stable interfaces.
- Prefer simplicity unless complexity is justified.
- Design for long service life.

### Linux and BSD Traditions

Unix, BSD, and Linux systems demonstrate practical systems engineering, text-based tooling, simple interfaces, and strong respect for portability.

Adopted principles:

- Plain text is a strength.
- Tools should compose.
- Interfaces should be documented.
- Avoid unnecessary dependencies.
- Prefer mechanisms over policy where appropriate.

## AEMS and Atarix Standard Position

AEMS and Atarix will use a C-first engineering style influenced by these projects while remaining its own standard.

The standard shall emphasize:

- C23 where useful, with portability boundaries documented.
- Clear headers and explicit public APIs.
- Tests for public behavior.
- Warnings treated seriously.
- Minimal hidden allocation.
- Minimal global state.
- Deterministic behavior where practical.
- Explicit error handling.
- Documentation as part of the deliverable.

## Not a Blind Copy

This standard does not blindly copy curl, Git, SQLite, Linux, BSD, or any other project. When their practices conflict, AEMS and Atarix choose the rule that best supports clarity, portability, safety, and long-term maintenance.

## Citation Notes

This document records influence and design intent. Specific technical rules should cite their upstream inspiration when a rule is directly derived from another project's published guidelines.
