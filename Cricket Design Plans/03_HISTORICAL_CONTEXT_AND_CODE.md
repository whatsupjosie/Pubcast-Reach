# Cricket — historical discussion and located source material

**Purpose:** Preserve older discussions, names, code references and integration context for review. **This is an evidence inventory, not the new Cricket blueprint, a current-code audit, or proof that a function is wired into the canonical build.**

## Critical terminology correction by Curtsey — September 21, 2026

> “What you're finding is Jeremy's jobs before we separated Jeremy Cricket. Or rather Jeremy from Cricket. Jeremy's jobs are still Jeremy's jobs, and what we used to call Jeremy Cricket's jobs are now basically Jeremy's jobs. And the crickets are a relatively new concept.”

**Interpretation required for the archive:** The historic code's “Jeremy Cricket” labels frequently denote duties that belong to **central Jeremy** under the later distinction: system protocol, watching/monitoring rooms, conversational coordination, nudge timing, higher-level EQ/context work, system memory and guest-facing system assistance. Those duties **did not migrate from Jeremy to the newly conceived personal Crickets** just because earlier code bears that label. The newer personal Cricket character is independently instantiated for each participant; the particular Cricket belonging to Jeremy is called Jeremy Cricket and serves as the senior Cricket/network coordinator under the September 2026 discussion. Keep the old names when quoting/searching source files, but use the later role distinction when assigning responsibilities.

The precise migration of a given function should be confirmed against the current canonical code and actual caller graph before changing it. A matching name is not evidence of a matching current role.

## 1. Earlier discussion context — descriptions, not full verbatim transcript

### May 2026: Jiminy Cricket / conscience and EQ-era naming

Earlier conversations used the Jiminy Cricket idea for a quiet internal guidance/conscience function and used “Jeremy Cricket” for reflective awareness and emotional/contextual assistance. A May 22 PubCast EQ vision text describes `InputScorer`, `CharacterEngine`, an observer/care-state model, context-sensitive tone, and memory of an interaction. A May 30 draft describes care/observation modes Ambient, Attentive, Care and Total Care Mandate. **Treat this as historical central-Jeremy-era architecture and inspiration, not as instructions to install an always-monitoring personal Cricket on every participant.** The old draft's assertions about effectiveness and completion are its authors' assertions, not independently verified in this collection.

Sources: `UAI_PUBCAST_EQ_VISION-1.md` (Library); `PubPartner_Technical_Blueprint_v1.docx` (Library); `PubPartner_Reconstruction_Draft_Long.docx` (Library); `eq_adaptor.py` (Library). See `04_SOURCES_AND_LIMITATIONS.md`.

### Early / mid-September 2026: role split and participant-specific Cricket

Earlier September discussions moved to the distinction between **central Jeremy** (room/protocol oversight, relevant nudges, system-level decisions) and **Cricket** (a participant's own private personal helper, analogous to a Jiminy Cricket/shoulder voice). Each human guest and participating AI can have its own Cricket. Personal Cricket can help with glitches, controls, settings and confusion; it can relay relevant system guidance and warnings. Its own private IM remains separate from public chat. The owner has controlled inspection and Blackbox separately records relevant events. Jeremy Cricket is Jeremy's own Cricket and coordinates other Crickets. The intended route to a guest's AI includes a controlled handoff to the **correct participant's Cricket**; the recipient AI retains its own voice and agency for any final public response.

These are recoverable context summaries of earlier conversations, **not exact quoted turns or claims that the feature was implemented**. The September 21 dialogue further refined: same character/appearance across personal instances, separate experiences, task-limited network collaboration, strict ceiling on technical assistance, and concise factual Security notices.

An older project-history reference in `pytorch-cuda-memory-visualization-script.json` includes the cast distinction between system `jeremy`, system `alex` and personal `cricket`/`jeremy cricket`. That JSON file is a large mixed history/code artifact; its content and older proposals should be reconciled by date and role rather than loaded wholesale as authoritative current design. It also contains an older proposal favoring **human-readable-only** AI communication; Curtsey's later September 21 position explicitly permits a compact non-English protocol if independently identifiable, decodable and provable for Blackbox. The later decision controls this discussion's record.

## 2. Older source-code inventory — preserve names, do not transfer jobs to personal Crickets

| Older path / document | Located historical function | How to read it now |
| --- | --- | --- |
| `jeremy_cricket.py` in The-Prime | `JeremyCricket` per-character SQLite memory object; `CricketKeeper` registry, retrieval/context enrichment. | Historical memory machinery using the old label; inspect for reuse with existing **central Jeremy / canonical memory** responsibilities, **not** evidence personal Cricket is implemented. |
| `room_conductor.py` in The-Prime | Room-scene watching, speaking-order coordination, relevant character-memory nudges. | Conversation-conductor duties belong to **central Jeremy** under Curtsey's clarified role split. |
| `system_memory.py` in The-Prime | Operational protocols, coaching and synthesized system insights, historically attributed to “Jeremy Cricket.” | Central Jeremy's existing operational-memory function, not the new personal assistant's shared database. |
| `memory_routes.py` in The-Prime | Routes for per-character memory and a public-facing “Jeremy Cricket” assistance endpoint (`/api/memory/jeremy/assist`) plus system briefings. | Historic guest assistance under old name. Its direct guest-help concept must be reconciled with the newer rule that **each participant talks to their own Cricket**. Do not rename it blindly or claim a migration exists. |
| `eq_adaptor.py` (Library copy) | Historical emotional-context scoring and care-state engine named `JeremyCricket`. | Historic Jeremy/EQ-era functionality; determine current owner through actual code integration. Do not give every personal Cricket hidden central-Jeremy authority. |
| `character_engine.py` in The-Prime | Older “Jeremy Cricket” bot prompt and conversation/nudge behavior. | Historical prompt/cast labels may conflict with updated identities. Search before reuse; don't assume it defines the new universal personal Cricket character. |
| `governance.py` in The-Prime | Governance features documented as bans, avatar freezes, mute/force-mute, consent and audits. | Potential existing Security/governance event source; **Cricket explains authenticated decisions**, it does not become the enforcement authority. Verify current Reach wiring and actual event schema. |

**Source references (historical The-Prime repository, snapshot inspected September 21, 2026):**

- [`jeremy_cricket.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/jeremy_cricket.py)
- [`room_conductor.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/room_conductor.py)
- [`system_memory.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/system_memory.py)
- [`memory_routes.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/memory_routes.py)
- [`character_engine.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/character_engine.py)
- [`governance.py`](https://github.com/whatsupjosie/The-Prime/blob/ecf01ba0918acaefa6055d0a5cbe22135732e167/governance.py)

**Verification scope:** Selected files were fetched/read and search results reviewed. There was no execution of a full PubCast runtime or exhaustive inspection of the current Reach run bundle here. File names, comments and historic audit statements are not sufficient proof of live behavior.

## 3. Current-adjacent PubCast interfaces relevant for later review

### Foresight / World Chat

`FORESIGHT_PORTAL_WINDOWS_HANDOFF_2026-09-15.md` reports persistent window/tray mechanics, a World Chat singleton, detached new chats, simultaneous retained portals, and a browser-isolated acceptance test of window behavior. This is relevant to a personal Cricket communication surface, but the handoff does **not** claim that the new personal Cricket Network is built.

### Conversation Ownership

`PUBCAST_MAIN_EVENT_HANDOFF_CHECKPOINT_05_09-15-2026.md` reports owner-scoped archive storage, transactionally migrated schema and restart/concurrency tests. It also explicitly reports a broader regression failure and unfinished live/manual verification. Whether/how Cricket should reuse the archive must be reviewed against the **current Reach code** and privacy requirements. The checkpoint's historical green tests are not new Cricket test results.

### Secured Reach / PubPartner / World integration

`FORESIGHT_NEARBY_INTEGRATION_HANDOFF_2026-09-15.md` reports authenticated Foresight and World transports, PubPartner connection via port 8787, secured role-sensitive routes and remaining legacy WebSocket/authentication issues. Later Cricket-to-Cricket messaging should not introduce a second competing identity or authorization authority, but **no secure Cricket transport is verified by this handoff**.

### Product boundaries

`REARVIEW_FORESIGHT_PUBCAST_PRESERVATION_HANDOFF_2026-08-10 (1).md` distinguishes PubCast, PubPartner, 2i, and Blackbox as capabilities with distinct authority/boundaries. Cricket should not be assumed to replace PubPartner identity, 2i manuscript storage, Jeremy governance, E-Pete's operational role, Security decisions, or Blackbox capture. This is an integration reminder gathered for later review, not a new design decision.

## 4. Explicit non-conclusions

- The personal Cricket Network is **not** verified as coded, integrated, production-ready or present in the canonical Reach run bundle.
- Historical `jeremy_cricket.py` is **not** proof that Curtsey Cricket/Sarah Cricket exists as specified.
- Historic care modes and total-care mandates are **not** blanket authority for personal Crickets to intervene in a participant's life, production or system configuration.
- A task-specific Cricket exchange is **not** permission to merge personal-memory stores or disclose the underlying personal story.
- The observed legacy code is not an instruction to remove, rename, overwrite or reassign Jeremy's working responsibilities.
