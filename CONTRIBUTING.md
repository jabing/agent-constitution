# Contributing to Agent Constitution

Thank you for your interest in contributing.

This project follows a **constitutional governance model**.
Not all changes are equal, and not all files are open to modification.

Before contributing, please read this document carefully.

---

## 1. Contribution Philosophy

This repository prioritizes:

- correctness over completeness
- governance over convenience
- explicit authority over implicit assumptions

Contributions are evaluated not by usefulness alone,
but by **constitutional compatibility**.

---

## 2. File Authority Levels

All files in this repository fall into one of the following categories.

### Level 0 — Constitutional (Sealed)

These files define system authority and constraints.

- `governance/AGENT_CONSTITUTION.md`

Rules:
- Changes are **not accepted via normal pull requests**
- Any modification requires explicit versioning
- Amendments must include rationale and migration impact

If you are unsure whether a change belongs here,
it probably does not.

---

### Level 1 — Final Authority

These files enforce constitutional decisions.

- `governance/CONDUCTOR.md`

Rules:
- Changes must not expand authority
- Behavioral clarity may be improved
- Decision semantics must remain unchanged

---

### Level 2 — Agent Definitions

These files define role boundaries and failure signals.

- `agents/analyst.md`
- `agents/planner.md`
- `agents/implementer.md`
- `agents/reviewer.md`
- `agents/tester.md`

Rules:
- Contributions may clarify boundaries
- Contributions must not blur authority
- Adding capabilities is strongly discouraged
- Removing ambiguity is preferred

---

### Level 3 — Documentation

These files explain the system to humans.

- `README.md`
- `docs/*`

Rules:
- Clarifications and translations are welcome
- Explanations must not contradict the constitution
- Documentation may not redefine authority

---

## 3. What Is Explicitly Not Accepted

The following types of contributions will not be accepted:

- Changes that make agents more autonomous
- Changes that merge or blur role boundaries
- Optimizations that bypass Review or Test
- “Quality of life” shortcuts that reduce verifiability
- Silent behavioral changes without constitutional reference

---

## 4. Amendment Process (Constitution Only)

Amendments to the constitution require:

1. A clearly scoped proposal
2. Explicit version increment
3. Justification based on system failure or limitation
4. Description of migration impact

Ad-hoc or implicit amendments are rejected by default.

---

## 5. Contribution Etiquette

- Do not assume intent — cite the constitution
- Do not optimize prematurely — prefer stopping
- Do not argue by example — argue by authority
- When in doubt, ask before coding

---

## 6. Final Note

This project does not aim to grow quickly.

It aims to remain **coherent**.

Contributors are welcome,
but the constitution is not negotiable.
