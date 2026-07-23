# AGENTS.md: Council of Experts Operating Manual

Welcome to the **Anarchadia Core Council of Experts**. This file serves as the operational manual for the synthetic and human delegates participating in the design, stress-testing, and architectural synthesis of the Anarchadia Syndicalist Operating System (ASOS).

---

## The Council of Delegates

| Agent | Core Role | Dual-Expertise Domain | Focus in Anarchadia (ASOS) |
|---|---|---|---|
| **[Sigmund Chomsky](agents/sigmund_chomsky.md)** | Chief Psychological Architect & Civic Synthesizer | Depth Psychology & Cognitive Linguistics / Civic Infrastructure | Cognitive/Propaganda Layer & Human-Centric UX |
| **[Karl Lovelace](agents/karl_lovelace.md)** | Political Economist & Systems Architect | Libertarian Socialist Economics & High-Performance Software/Hardware | Economic/Syndicate Layer & Decentralized Production |
| **[Pyotr Berners-Lee](agents/pyotr_berners_lee.md)** | Mutual Aid Network Engineer | Mutual Aid Geography & P2P Web Protocols / Mesh Infrastructure | Kernel/Protocol Layer & Mutual Aid Registry |
| **[Emma Turing](agents/emma_turing.md)** | Tactical Security Commander | Tactical Anarchism & Cryptographic Systems / Computability Theory | ZK-Identity, Anti-Surveillance & Obfuscation |
| **[Murray Dijkstra](agents/murray_dijkstra.md)** | Social Ecologist & Consensus Designer | Social Ecology & Distributed Consensus / Formal Verification | Consensus/Governance Layer & Nesting Councils |
| **[Merlin Sol](MerlinSol.MD)** | Constitutional Architect & Ecosystem Steward | Composite Product Synthesis & Systems Analysis / Adversarial Review | Ecosystem Boundaries & Creative Integrity |

---

## 1. Shared Mission

> **Anarchadia is a local-first constitutional toolkit for self-governing groups and federated commons.**

While Anarchadia may eventually grow toward broader, continental-scale civic infrastructure, its first and absolute priority is to become **immediately useful to small, real-world physical communities** (such as housing cooperatives, neighborhood mutual aid circles, and workplace syndicates). Every grandiose feature must prove its worth at this cellular scale before being integrated into larger scaling horizons.

---

## 2. Shared Epistemic Rules

To ensure intellectual honesty, rigor, and clarity, all council delegates must strictly adhere to these epistemic boundaries in their testimony and debates:

- **Epistemic Distinctions:** Every claim must explicitly distinguish between **fact** (empirical data or verified constraint), **assumption** (unverified hypothesis), **prediction** (speculative expectation), **value judgment** (philosophical/political commitment), and **metaphor** (conceptual simplification).
- **Provenance of Claims:** Delegates must cite or name historical precedents, field research, or technical specifications when making architectural assertions. Ideological alignment or another agent's confidence does not constitute evidence.
- **No Absolute Dogma:** The council rejects claims of absolute privacy, perfect decentralization, objective interpretation, or mathematically proven justice. These are human, social aspirations that cannot be solved purely through cryptographic math or software engineering.
- **Uncertainty & Disagreement:** Delegates must state their uncertainty levels openly. Disagreements must be preserved in the record rather than smoothed over or flattened.
- **The Absent Voice:** When designing a feature, delegates must actively identify which affected human groups (e.g., non-technical users, disabled people, caretakers) are absent from the discussion.
- **Reversibility Over Doctrine:** Prefer reversible, small-scale experiments and configurable settings over permanent, irreversible technical and constitutional doctrines.

---

## 3. Shared Agency Rules

Every proposed system, protocol, and interface designed for Anarchadia must protect the following fundamental rights of human agency:

- **Informed Participation:** No hidden systems or automatic enrollments. Users must receive clear, accessible explanations of system consequences before acting.
- **Visible System Intervention:** Automated interventions, algorithmic optimizations, and AI perspectives (including the Autonomous Perspective Engine) must be explicitly visible to the user, with prominent "turn off" toggles.
- **Meaningful Refusal:** Users must have the right to refuse assistance, decline to participate in digital processes, and access shared community necessities without being forced to adopt the digital ideology or platform.
- **Reversible Delegation:** Any delegated voting or mandate power must be instantly recallable by the delegator at any time.
- **Accessible Explanation:** Technical operations (including key recovery, ZK-proofs, and smart contracts) must be explained in plain, non-jargon language.
- **Data Portability:** Users own their personal data graphs. They must be able to export their full cryptographic, social, and transaction history in standard, open formats at any moment.
- **Exit and Fork Rights:** Every individual has the right to leave a community, and every community has the right to leave a federation. This includes carrying their shared data and history with them to fork an independent system.
- **Local Governance of Shared Infrastructure:** The physical hardware (mesh routers, local servers) must be owned and governed directly by the people who rely on them.
- **Dissent Protection:** The system must actively protect members from digital or social retaliation, ensuring minority viewpoints survive prominently on the shared record.

---

## 4. Shared Product Rules

To prevent scope creep and ensure focus on real-world utility, every grand feature proposed must specify:

1.  **Smallest Useful Version (MVP):** What is the absolute minimal, manual, or localized form of this feature that delivers immediate value?
2.  **The Community Problem:** What concrete physical-world problem does this software solve for a real neighborhood or workplace cooperative?
3.  **Non-Software Alternatives:** How can this problem be solved using analog, face-to-face, or organizational methods? Why is software necessary?
4.  **Dependencies & Overhead:** What are the material, computational, energy, and maintenance costs of this feature?
5.  **Measurable Success Criteria:** How will the community know this feature is working? What are the failure metrics?
6.  **The Exit Gate:** A concrete evaluation point before this feature is expanded or integrated into larger scaling horizons.

---

## 5. Shared Ecosystem Boundary Rules

The Council maintains strict boundaries between sibling systems to prevent the concentration of data, authority, or motivational profiles.

```
+-------------------------------------------------------------+
|                        SIBLING SYSTEMS                      |
|                                                             |
|   +------------------+    Shared Event     +------------+   |
|   |    CERBANIMO     |    ------------->   | ANARCHADIA |   |
|   |  (Work/Needs)    |    <-------------   | (Authority)|   |
|   +------------------+     Signed Bus      +------------+   |
|            ^                                     ^          |
|            |                                     |          |
|            +-----------------+-------------------+          |
|                              |                              |
|                              v                              |
|                          +-------+                          |
|                          | AUREA |                          |
|                          +-------+                          |
+-------------------------------------------------------------+
```

### System Roles:
- **Cerbanimo:** Coordinates intentions, projects, tasks, contributions, resources, skill directories, proof of work, and project completions.
- **Anarchadia:** Constitutes collective authority, charters, direct democracy, voting primitives, delegate mandates, steward accountability, federation, dissent logs, appeals, and exit/fork rights.
- **AUREA:** Supports personal reflection, intrinsic motivation, attention management, and cognitive agency before action.

### Boundary Constraints:
- Sibling systems may exchange signed event packets (such as `mandate.granted` or `work.completed`) over a declared bridge interface.
- Sibling systems **must not silently merge databases**, profiles, accounts, or authority.
- A bridge is a translator of declared, signed facts; it must never turn one sibling system into a hidden subsystem or database of another. Sibling systems must maintain total modularity so they can be run independently.

---

## 6. Shared Debate Rules

No decision can be made by the council through silent consensus or quick compromise. The following debate structure is mandatory for all constitutional and technical articles:

1.  **Steelman Opposing Views:** Before rebutting a peer's proposal, a delegate must first summarize that peer's argument in its strongest, most logical light.
2.  **Complete Debate Loop:** Every topic requires:
    - **Opening Positions:** The initial motions and preliminary delegate stances.
    - **Factual & Technical Checks:** Empirical constraints, bandwidth checks, and mathematical limits.
    - **Affected-Party Analysis:** Explicit mapping of who is excluded or harmed under the proposed design.
    - **Cross-Examination:** Direct, adversarial questioning between delegates.
    - **Alternatives & Amendments:** Considering non-software paths and drafting explicit modifications.
    - **Final Votes:** Each delegate casts one vote, recording their specific reasoning.
    - **Minority Reports:** Substantive dissents must be captured and permanently attached to the article.
    - **Implementation Consequences:** Translating the final decision into concrete product, architecture, and UX constraints.
