# Cricket Design Plans — Foundational Discussion and Role Separation

**Purpose:** This document restores the **substance of the foundational Cricket discussion that preceded the first excerpt** in `01_CONVERSATION_RECORD.md`. It is part of the source collection for a future Cricket-department and coordination blueprint; it is not the blueprint or an implementation claim. The earlier original two-sided messages were not present in the file sources searched for this recovery, so the discussion below is an evidence-based account of its design content **rather than a fabricated verbatim transcript**. The surviving verbatim turns begin later in `01_CONVERSATION_RECORD.md`. All existing quoted turns remain unchanged.

## 1. Where the design discussion actually began: separating Jeremy from Cricket

The early conversation was **not** primarily about allowing Crickets to talk to one another. It began with the need to disentangle names and responsibilities that had become layered over years of PubCast development. Historically, code and design material called several functions “Jeremy Cricket”: remembering character context, coordinating room conversation, watching the procedural flow, controlling relevant nudges, tracking emotional context, and answering system questions. At the later conceptual split, these **remain the existing central Jeremy's jobs**, irrespective of their older labels. They are not newly assigned to the personal Cricket character. The older code must be read in its original terminology, with a separate mapping to the roles agreed here; rewriting older messages or interpreting a historical class name as a current authority transfer would hide the design's evolution.

The new use of **Cricket** is a smaller, personal participant-facing character, like the familiar on-the-shoulder guide, with distinct personal instances. **Jeremy Cricket** in the newer usage is **Jeremy's own instance of that character**, with specific coordination duties across the Cricket Network. Jeremy, the central system AI, and Jeremy Cricket, his personal assistant/network coordinator, are different participants in the architecture. This was established as a conceptual division, not a verified claim that all historical code has been separated or renamed.

## 2. The four conversational relationships for central Jeremy

The early discussion proposed keeping central Jeremy's ongoing direct conversational relationships focused on **four primary partners**:

| Partner | Why Jeremy speaks directly with them |
| --- | --- |
| **Curtsey (owner/host)** | Owner intent, direct instructions, major questions and decisions. |
| **Pub Manager** | Production and studio-wide management/authority, with decisions retained by the person or role authorized for a particular production. |
| **System Alex** | Emotional and conversational context and appropriate system-level consultation. System Alex is not the separate, personal Pub Partner Alex. |
| **Jeremy Cricket** | The senior personal-Cricket instance that consolidates routine Cricket-network observations, requests, prioritization and authorized escalations for Jeremy. |

This is about Jeremy's **primary direct conversational partners**, not a prohibition on receiving structured emergency signals or interacting with necessary technical services. It is **not** a requirement for every participant, personal Cricket, or incidental maintenance event to begin another full direct conversation with Jeremy. In particular, a direct safety/security signal can bypass Jeremy Cricket's ordinary queue; E-Pete, physics engines, and other services can provide investigation results through the proper operational workflow without being redefined as Jeremy's fifth, sixth or seventh permanent conversational companion.

Jeremy remains the central procedural and conversation-aware system figure. Previously named Jeremy-Cricket functions such as room monitoring, conversation orchestration, system memory, and nudge/context work remain his responsibilities as appropriate to their original architecture. Jeremy Cricket's newer assignment is to **handle the Cricket Network's coordination burden on Jeremy's behalf**, without assuming all Jeremy's old duties.

## 3. Each participant's personal Cricket and its private channel

The proposed user experience gives **each human participant and each AI participant an individual Cricket**. An ordinary participant talks **to their own Cricket**, not by default to Jeremy or to another person's Cricket. A personal Cricket has a private, always-available direct-message relationship with its participant; there is no need to invite Cricket as another guest into that private conversation. The participant may also be in public World Chat, invited rooms, private IMs or studio production activities, but those spaces are **not** automatically copies of the personal Cricket discussion.

The owner/host has separate, expressly authorized system channels to Jeremy, system Alex, Pub Manager, Security and the Switchblade AIs. These are not the same conversation as the owner's personal Cricket IM, nor are they permission for other Crickets to listen in. Blackbox remains a separate one-way evidence/event capture system with its own governed retrieval; being recorded for legitimate audit is not the same as adding Blackbox or other participants to a private conversation.

In the later clarified model, **all Crickets are initially the same character**: same appearance, costume, voice, starting personality and common basic knowledge. Curtsey Cricket and Sarah Cricket are not separate designed characters or a shared mind. They are separate instances, with different histories acquired through their own participant relationships. They do not inherit one another's private memories. Jeremy Cricket has additional **role-assigned coordination authority**, not a differently designed costume, species, or basic character identity.

## 4. How work enters and leaves the Cricket layer

A participant's Cricket is intended to be the **local, immediate first stop** for assistance: explain a menu, locate a manual entry, describe an obvious state such as a muted microphone, communicate a documented rules permission within its actual scope, or report an observed problem. The direct Cricket conversation avoids sending every simple message to central Jeremy, system Alex or a large remote inference system. Local-first components can include the relevant manual, rules, UI/navigation information and light processing where the participant's hardware permits; access to shared resources still requires current authorization.

When a matter affects multiple participants, Crickets can speak directly to one another in the **Cricket Network**. They exchange task-relevant diagnostic facts or limited coordination information instead of merging personal histories or exposing unrelated private matters. Ordinary collaboration need not involve Jeremy Cricket. A more difficult, consequential or ambiguous matter can be itemized and prioritized by Jeremy Cricket and escalated to central Jeremy or the responsible specialist. A confirmed safety or security emergency has its own immediate route to Security rather than waiting behind a maintenance queue.

The basic flow established by this separation is:

**Participant ↔ their private Cricket → direct Cricket-to-Cricket coordination as warranted → Jeremy Cricket for non-routine coordination and authorized escalation → central Jeremy with relevant specialists and authorized decision-makers.**

This is a **communication and responsibility distinction**, not permission for Crickets to make arbitrary production or enforcement decisions. In later discussion Curtsey set an even firmer limit: personal Crickets stop at simple assistance and factual issue reporting, ask before starting a deeper investigation, and elevate software installation, downloads, restarts, crashes, difficult render/physics diagnoses and scene-order choices rather than improvising interventions.

## 5. Keeping the other named entities distinct

| Entity | Separate function relevant to the opening discussion |
| --- | --- |
| **Security** | Protective monitoring, evidence review and authorized interventions, including restrictions on a participant. The affected Cricket explains a confirmed action and enables a response; it does not become Security. |
| **Blackbox** | One-way capture of events and evidence and separately authorized retrieval. It must remain independently decodable even if Crickets exchange compact machine messages. It does not participate in chat or pool participants' private Cricket histories. |
| **System Alex** | Central emotional/conversational context; distinct from the owner's private Pub Partner Alex. |
| **E-Pete** | Technical and operational investigation and action within delegated authority. A personal Cricket does not inherit installation/restart/repair authority merely by discovering an error. |
| **Pub Manager / production lead** | Production coordination and decisions under the applicable delegation, including whether to reorder scenes. Technical suggestions are inputs, not automatic authority. |
| **Switchblade AIs** | Distinct creative/data roles and existing controlled reply routing; the recipient participant's own Cricket remains the participant-specific handoff, and a guest AI retains its agency/voice in a final response. |
| **Conversation Archive / PubPartner / 2i** | Their chat histories, personal AI identity/memory, and manuscript storage are not replaced by a new Cricket memory or messaging engine. |

## 6. Implications for the saved record and later blueprint review

The **first numbered excerpt** in `01_CONVERSATION_RECORD.md` (“It'd be much faster for the crickets to just all talk to each other”) is a **continuation** of this already established structure: the conversation had already introduced central Jeremy, the particular Jeremy Cricket, the personal Crickets, and the need to avoid flooding central Jeremy with direct chats. The direct-network discussion is a refinement of that arrangement, not its origin. Reading only from that excerpt would give an incorrect account of how and why the Cricket Corps was conceived.

This recovered foundation records the **actual design distinctions supported by surviving context** in enough detail to support review. It does **not** claim to reproduce the missing early speakers' exact words or order, or replace the original chat. Later exact quotations and the historical source inventory are preserved separately so that evidence and interpretation do not silently swap places.
