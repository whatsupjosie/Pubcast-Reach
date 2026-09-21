# Cricket Design Plans — sources, provenance and limitations

**Status:** Evidence register prepared for archival review, not a current build verification report.

## Source classes

**A. September 21, 2026 discussion in this ChatGPT conversation.** The user turns appear verbatim in `01_CONVERSATION_RECORD.md` in chronological order. The assistant response blocks in that file are explicitly labeled editorial recaps, because this workflow did not retrieve an official machine-readable message export or reproduce every complete assistant answer and rendered diagram. The original ChatGPT conversation is the authoritative source for the exact full dialogue. No original chat messages were altered by producing this archive.

**B. Earlier ChatGPT conversation context.** Prior discussions about Jeremy/Cricket and a September 15 role split informed the historical notes. They were available as conversation-history summaries, not a complete verbatim prior-chat export. The archive does not fabricate quotation marks or timestamps for missing original turns. Earlier context is labeled as summary.

**C. Retrieved Library files.** The following identifiable sources were discovered and inspected using the user's file library. They are source material, not newly generated Cricket deliverables:

- `PubPartner_Technical_Blueprint_v1.docx` (May 30, 2026) — older PubPartner/EQ observer, evidence-layer and memory-cartridge concepts; Library retrieval marker `turn17file0` at collection time.
- `PubPartner_Reconstruction_Draft_Long.docx` (May 30, 2026) — earlier observer/care-state framing; retrieval marker `turn8file0`.
- `UAI_PUBCAST_EQ_VISION-1.md` (May 22, 2026) — earlier EQ/voice/care descriptions, including historic naming and claims of prior tests; `turn18file2`.
- `eq_adaptor.py` (Library, found September 21, 2026) — older care-scoring `JeremyCricket` class; `turn18file0`.
- `pytorch-cuda-memory-visualization-script.json` (Library, large mixed content file) — historical embedded PubCast cast/code context. Not audited exhaustively.
- `FORESIGHT_PORTAL_WINDOWS_HANDOFF_2026-09-15.md` — Foresight windows, World Chat lifecycle and partial verification; `turn17file2`.
- `PUBCAST_MAIN_EVENT_HANDOFF_CHECKPOINT_05_09-15-2026.md` — conversation archive schema/recovery tests, open regression and remaining gaps; `turn17file1`.
- `FORESIGHT_NEARBY_INTEGRATION_HANDOFF_2026-09-15.md` — secured Foresight and PubPartner/8787 integration evidence with stated limitations; `turn17file7`.
- `REARVIEW_FORESIGHT_PUBCAST_PRESERVATION_HANDOFF_2026-08-10 (1).md` — product-boundary and integration context; `turn8file6`.

Retrieval markers are internal to the collection session and may not function as durable links when this folder is later opened independently. Search by the exact filenames above in the user's Library.

**D. Historical GitHub code.** The-Prime `jeremy_cricket.py`, `room_conductor.py`, `system_memory.py`, `memory_routes.py`, `character_engine.py` and `governance.py` were fetched in this collection. Immutable commit links appear in `03_HISTORICAL_CONTEXT_AND_CODE.md`. They are older sources, **not** an audit of the currently running canonical Reach distribution.

## Corrections, scope and authority

1. **Later Curtsey clarification overrides misleading old names.** Prior “Jeremy Cricket” system-memory, room-conduction, rule-monitoring and conversation-coordination jobs generally belong to **central Jeremy** after the conceptual split. The new personal Cricket character and the particular instance belonging to Jeremy are newer concepts. Keep the historical code names for provenance only.
2. **Keep user decisions separate from assistant proposals.** A suggestion about autonomous scene planning, extensive Cricket authority, always-on observation, or a user-interface design is not accepted simply because it appeared in an assistant reply. Curtsey later narrowed the personal Cricket role to simple local help, factual reporting and authorized escalation.
3. **Retain the rejected network name only as a historical quote.** The working name is Cricket Network.
4. **No claim of full transcript export.** The user asked for the entire conversation. This collection preserves all user turns accessible here, with assistant-topic recaps, but **does not satisfy word-for-word preservation of every assistant turn**. Obtaining the native ChatGPT conversation export is necessary for that exact fidelity. This limitation is disclosed rather than silently paraphrasing as a verbatim transcript.
5. **No build or test claim.** No Cricket source was changed, no canonical run bundle was launched or audited, and no production tests were executed for this collection.
6. **No external project modifications.** This archival work does not push to GitHub, alter a connected source document, or redefine the current live PubCast behavior. It creates a separate Markdown folder in the working container, intended for the user's file Library.

## Suggested review order (not a design plan)

Read `01_CONVERSATION_RECORD.md` for chronological user decisions and their surrounding assistant ideas; read `02_GATHERED_DESIGN_NOTES.md` for a concise topic index; consult `03_HISTORICAL_CONTEXT_AND_CODE.md` for the older Jeremy naming issue and source leads; consult this file to understand what is source-backed, summarized, superseded or still unavailable verbatim.
