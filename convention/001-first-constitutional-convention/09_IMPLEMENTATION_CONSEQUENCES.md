# Consolidated Implementation Consequences

## Article 1: Purpose, Identity, and Non-Goals

- **Product constraints:** Product must focus strictly on local group coordination (charters, proposals, decisions).
- **Architecture constraints:** Rust core, libp2p local transport layer, zero cloud backend dependencies.
- **Data constraints:** Local SQLite storage replicated via P2P CRDTs.
- **Security constraints:** Local device database encryption by default.
- **UX constraints:** No infinite scroll, no push notifications, positive friction prior to high-impact votes.
- **Explicit non-goals:** No global cloud synchronizer, no bare-metal drivers.
- **Candidate work packets:** Implement local GossipAid Wi-Fi syncing prototype; design JSON-LD group charter schemas.

---

## Article 2: Human Agency and Voluntary Association

- **Product constraints:** Include 'Print Paper Ledger' and 'Manual Transcription' workflows in the MVP UI.
- **Architecture constraints:** Event-based database design allowing batch-processing of manual entries.
- **Data constraints:** Database schema must support data-stripping (anonymization) of deleted user nodes without breaking chain integrity.
- **Security constraints:** Implement cryptographic pruning of private association metadata upon exit.
- **UX constraints:** Provide a simple, non-shaming 'Offline User' status option.
- **Explicit non-goals:** Do not build automated tracking of offline users; manual data entry must remain community-driven.
- **Candidate work packets:** Create a data migration and schema-export tool; design a manual entry synchronization pipeline.

---

## Article 3: Membership, Identity, Pseudonymity, and Recovery

- **Product constraints:** Include 'Vouch for Neighbor' and 'Social Key Recovery' wizards in the core identity module.
- **Architecture constraints:** Implement shamir secret-sharing library optimized for mobile compilation.
- **Data constraints:** Separate public qualification tokens from private relational profiles in the storage schema.
- **Security constraints:** Enforce zero plaintext key transit; all recovery packages are encrypted locally before sharing.
- **UX constraints:** Provide visual indicators showing the strength of a user's local social backup network.
- **Explicit non-goals:** Do not integrate global federated KYC or single sign-on systems.
- **Candidate work packets:** Implement local social secret sharing prototype; write ZK membership verification tests.

---

## Article 4: Rights of Persons and Duties of Institutions

- **Product constraints:** Include 'Rights Checklist' and 'Dissent Attachment' features into the MVP assembly module.
- **Architecture constraints:** Implement net-neutral packet prioritization and local, cryptographic token-bucket rate limiting.
- **Data constraints:** Enforce strict data separation between public accountability logs and private personal communication.
- **Security constraints:** Enforce zero-knowledge validation ciphers for all assembly votes.
- **UX constraints:** Provide a simple, prominent button to attach a dissent note to any passed proposal.
- **Explicit non-goals:** Do not build centralized moderator tools or content-censorship filters.
- **Candidate work packets:** Design the schema for permanent dissent attachments; implement local net-neutral routing test suite.

---

## Article 5: Transparency, Privacy, and the Commons

- **Product constraints:** Provide a split dashboard: 'My Private Ledger' (local and encrypted) and 'Community Commons Log' (public and shared).
- **Architecture constraints:** Integrate zero-knowledge credentials with cryptographically blinded transaction flows.
- **Data constraints:** Enforce strict separation between personal database tables (SQLite) and public gossip logs.
- **Security constraints:** Implement blind signature cryptography for all resource transactions.
- **UX constraints:** Provide visual indicators showing which transactions are public and which are fully blinded.
- **Explicit non-goals:** Do not build any centralized transaction tracing or user identity mapping engine.
- **Candidate work packets:** Implement a blind-signature test suite; design schemas for public inventory tracking.

---

## Article 6: Governance Primitives

- **Product constraints:** Include 'My Delegations' dashboard with instant recall button in the MVP.
- **Architecture constraints:** Implement CRDT-based event-ledger for vote tallying with vector clock ordering.
- **Data constraints:** Design relational schema mapping voting pools, delegation paths, and vote events.
- **Security constraints:** Enforce zero-knowledge proofs for voting credential validation.
- **UX constraints:** Provide real-time delegation graphs showing who holds delegated votes, with simple click-to-override.
- **Explicit non-goals:** Do not build un-recallable representative structures or permanent governance councils.
- **Candidate work packets:** Verify nested recall logic in TLA+; implement localized quadratic voting contract.

---

## Article 7: Delegation, Mandates, Administration, and Recall

- **Product constraints:** Include 'Steward Mandate Countdown' widget and 'Initiate Recall' action buttons in the MVP.
- **Architecture constraints:** Implement smart contracts with time-lock and automatic key-disabling functions.
- **Data constraints:** Design schemas tracking steward mandates, budgets, and recall transaction histories.
- **Security constraints:** Enforce strict key separation between public coordinating roles and private individual keys.
- **UX constraints:** Provide highly visible status displays showing who is currently performing a role and when it expires.
- **Explicit non-goals:** Do not build permanent administrative root accounts or un-recallable command roles.
- **Candidate work packets:** Implement automatic time-lock key expiration tests; write recall-block smart contracts.

---

## Article 8: Conflict, Harm, Safety, and Restorative Process

- **Product constraints:** Include 'Request Protective Separation' emergency action and 'Restorative Circle' charter wizard in the MVP.
- **Architecture constraints:** Implement local-only encrypted database vaults for dispute resolution records.
- **Data constraints:** Design schemas for restorative plans, separate from public transaction or identity logs.
- **Security constraints:** Enforce multi-key encryption (victim + mediator + assembly co-signers) for dispute data.
- **UX constraints:** Provide highly visible, accessible, non-confusing safety buttons with instant local device data-scrubbing.
- **Explicit non-goals:** Do not build public offender registries, automated credit penalties, or central ban tools.
- **Candidate work packets:** Write local encrypted dispute-vault prototypes; implement protective separation protocols.

---

## Article 9: Economic Coordination and Resource Stewardship

- **Product constraints:** Include 'Shared Inventory Log' and 'Gift Registry' modules in the core economic interface.
- **Architecture constraints:** Implement decentralized semantic web graph databases for local JSON-LD resource tracking.
- **Data constraints:** Design schemas mapping multi-asset balances, including labor hours, tools, and ecological footprints.
- **Security constraints:** Apply zero-knowledge blinding to all personal transaction ledgers.
- **UX constraints:** Provide highly readable, non-financial visual summaries of community resource abundance.
- **Explicit non-goals:** Do not build automated trading bots, interest engines, or secondary token markets.
- **Candidate work packets:** Design the JSON-LD economic schemas; write blinded mutual-credit ledger smart contracts.

---

## Article 10: Ecological Responsibility

- **Product constraints:** Include 'My Connection Status' dashboard and 'Add Community Relay' wizard in the MVP UI.
- **Architecture constraints:** Rust core running on-device SQLite database, interfacing with GossipAid (libp2p P2P transport).
- **Data constraints:** Separate encrypted local tables from public, signed event streams.
- **Security constraints:** Enforce end-to-end encryption for all data pushed to community relays.
- **UX constraints:** Provide a simple connection visualization showing if the user is 'Local-Only', 'Mesh Connected', or 'Gateway Connected'.
- **Explicit non-goals:** Do not integrate AWS APIs, centralized cloud database syncing, or mandatory global domain registries.
- **Candidate work packets:** Implement local SQLite database replication over direct Wi-Fi sync; write local NAT discovery tests.

---

## Article 11: Epistemic Commons and Media Interpretation

- **Product constraints:** Provide a simple P2P RSS and Markdown Note reader in the MVP suite.
- **Architecture constraints:** Implement decentralized feed replication over GossipAid.
- **Data constraints:** Design schemas for signed feed articles and user-configured feed subscriptions.
- **Security constraints:** Enforce local-only encryption of the user's reading history.
- **UX constraints:** Provide a clean, plain-text interface with zero gamified recommendation algorithms.
- **Explicit non-goals:** Do not build centralized feed servers, automated deprogramming prompts, or centralized moderator backoff controls.
- **Candidate work packets:** Design P2P feed syncing protocols; implement local feed-reading databases.

---

## Article 12: Technical Sovereignty and Architecture

- **Product constraints:** Include 'My Connection Status' dashboard and 'Add Community Relay' wizard in the MVP UI.
- **Architecture constraints:** Rust core running on-device SQLite database, interfacing with GossipAid (libp2p P2P transport).
- **Data constraints:** Separate encrypted local tables from public, signed event streams.
- **Security constraints:** Enforce end-to-end encryption for all data pushed to community relays.
- **UX constraints:** Provide a simple connection visualization showing if the user is 'Local-Only', 'Mesh Connected', or 'Gateway Connected'.
- **Explicit non-goals:** Do not integrate AWS APIs, centralized cloud database syncing, or mandatory global domain registries.
- **Candidate work packets:** Implement local SQLite database replication over direct Wi-Fi sync; write local NAT discovery tests.

---

## Article 13: Security and Threat Model

- **Product constraints:** Include 'Configure Duress PIN' and 'Social Backup Setup' wizards in the MVP security module.
- **Architecture constraints:** Rust cryptographic engine compiling to ARMv7-A and RISC-V targets.
- **Data constraints:** Enforce absolute physical database separation between standard profiles and plausible deniability profiles.
- **Security constraints:** Enforce zero plaintext caching of passwords, keys, or decrypted data in device memory.
- **UX constraints:** Provide a simple, non-technical security health check showing if the user's social backup is active.
- **Explicit non-goals:** Do not build global key escrows, cloud password managers, or developer recovery portals.
- **Candidate work packets:** Implement ARMv7-A cryptographic benchmark tests; write duress-wipe and plausible deniability profile tests.

---

## Article 14: Ecosystem Boundaries

- **Product constraints:** Include 'Configure Application Bridges' and 'Authorize Event' toggles in the MVP settings panel.
- **Architecture constraints:** Implement modular IPC (Inter-Process Communication) and event buses using signed capnproto or protobuf schemas.
- **Data constraints:** Enforce absolute physical database isolation between the SQLite instances of each application.
- **Security constraints:** Apply separate cryptographic key generation rules for each sibling package.
- **UX constraints:** Provide distinct, high-contrast visual themes for each application to prevent cognitive confusion.
- **Explicit non-goals:** Do not build single-database suites, unified identity trackers, or automatic multi-app sync agents.
- **Candidate work packets:** Design signed capnproto bridge event schemas; implement local IPC event-bus verification tests.

---

## Article 15: Federation, Subsidiarity, Exit, and Fork

- **Product constraints:** Include 'My Federation' topology map and 'Initiate Database Fork' action button in settings.
- **Architecture constraints:** Implement database-slicing and metadata-pruning algorithms for clean fork execution.
- **Data constraints:** Design schemas for federated event-logs and signed delegate mandate blocks.
- **Security constraints:** Enforce multi-party encryption for federated data-replication tables.
- **UX constraints:** Provide visual models of federated network as a network of equal rings with no pyramid structure.
- **Explicit non-goals:** Do not build representative legislative chambers, centralized tax collection modules, or permanent regional executive offices.
- **Candidate work packets:** Design federated database-slicing protocols; write delegate-revocation smart contracts.

---

## Article 16: First Useful Community

- **Product constraints:** Product MVP features are strictly locked to the five worker-coop journeys.
- **Architecture constraints:** Implement single-database per co-op design, running on SQLite on-device with peer-sync capability.
- **Data constraints:** Design schemas for co-op charters, member rosters, proposal logs, and transaction ledgers.
- **Security constraints:** Enforce local device database encryption and emergency data-scrubbing triggers.
- **UX constraints:** Provide a simple, clean, non-confusing dashboard showing 'Our Charter', 'Our Roster', 'Current Proposals', and 'Commons Ledger'.
- **Explicit non-goals:** Do not build multi-coop global directories, automated shipping routes, local token exchange markets, or bare-metal hypervisors.
- **Candidate work packets:** Implement local database initialization with worker co-op defaults; write emergency-wipe test suite.

---

## Article 17: MVP Constitution

- **Product constraints:** Product MVP features are strictly limited to the five worker-coop journeys; all other menus are hidden.
- **Architecture constraints:** Rust core with React Native frontend, SQLite local storage, direct Wi-Fi/Bluetooth sync.
- **Data constraints:** Design schema for local SQLite tables, isolating standard profiles from duress profiles.
- **Security constraints:** Apply standard libsodium and noise-protocol implementations.
- **UX constraints:** Provide a clean, plain-text dashboard focused strictly on local assembly operations.
- **Explicit non-goals:** Do not build custom microkernel drivers, local token markets, or automated regional supply routers.
- **Candidate work packets:** Create React Native build pipeline; implement local SQLite on-device database tests.

---

## Article 18: Amendment, Experimentation, and Ratification

- **Product constraints:** Include 'Constitutional Vote' module and 'View Local Patches' list in the MVP settings.
- **Architecture constraints:** Implement on-device schema-migration and constitutional patch loading engines.
- **Data constraints:** Design schemas tracking constitutional versions, active experiments, and signed ratification votes.
- **Security constraints:** Apply zero-knowledge voting verification for all human ratification sessions.
- **UX constraints:** Provide a simple, clean, non-technical dashboard showing the active rules, their sunset dates, and pending amendments.
- **Explicit non-goals:** Do not build developer backdoor switches, permanent default configurations, or automated enforcement of un-ratified rules.
- **Candidate work packets:** Implement local rule-change voting smart contracts; write local constitutional sunset test suite.

---
