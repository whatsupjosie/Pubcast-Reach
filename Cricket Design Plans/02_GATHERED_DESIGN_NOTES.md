# Cricket — gathered discussion notes (not a blueprint)

**Status:** Collection for review. These notes distinguish what Curtsey explicitly said from suggestions that the assistant introduced. For conversation order and original user wording, see `01_CONVERSATION_RECORD.md`.

## A. Character and personal-instance model — user decisions

- Cricket is **one consistent character**: every participant meets what appears to be the same character, with the same initial personality, appearance, costume and baseline knowledge. There is no bespoke personality or costume per participant.
- Each person or AI has its **own instance** and private relationship with that Cricket. Curtsey Cricket learns Curtsey’s experiences; Sarah Cricket learns Sarah’s experiences. Instances start identically and diverge slightly through their own participant interactions. The distinction is individual experience, **not** different character definitions.
- Personal histories do **not** automatically cross over. Limited shared experiences may occur when two Crickets collaborate on the same incident. They may retain the relevant outcome from their respective perspectives without importing each other’s private histories.
- A participant normally interacts with **their own Cricket**. They need not invite that Cricket into their existing private personal conversation. Each Cricket’s personal relationship remains private by default.
- Jeremy Cricket is **Jeremy’s personal instance** of the same Cricket character, assigned senior network coordination. Central Jeremy and Jeremy Cricket are separate. **Historical code named “Jeremy Cricket” performed duties that remained with central Jeremy after the later role split**; do not migrate those duties onto personal Crickets merely because of old names. System Alex and the owner's personal PubPartner Alex are also distinct.

## B. Communication — user decisions and examples

- Crickets are members of a shared **Cricket Network**. Curtsey expressly rejected the earlier name “NARC network”; do not revive it as a label.
- Crickets may talk directly to one another as needed. Jeremy Cricket can talk to all Crickets and coordinates matters that need wider help; ordinary conversations do not all pass through him.
- Cricket-to-Cricket communications are working conversations: problem-solving, troubleshooting, maintenance, safety, security and useful general information; also focused assistance relevant to a shared task or interaction.
- A Cricket may know private context about its own participant without sharing it. If relevant to collaboration, it can communicate only the minimum useful context: e.g. “Sarah is dealing with a personal matter and may need extra patience,” **not** the underlying personal story. The goal is to help the interaction, not spread the participant’s private life. Disclosure scope and the participant’s preferences remain important.
- Technical example: one Cricket reports checks A, X, Z and F negative and asks the other Cricket what the corresponding results were. They exchange diagnostic findings; they do not merge memories.
- Shared production example: one performer’s computer renders a car-crash scene slowly and lags the shared cue clock. Their Crickets compare actual local and cross-system telemetry. They may notice a possible scheduling workaround, but should not become production directors or automatically solve complex scheduling issues.

## C. The responsibility boundary refined over several turns

Curtsey refined the scope **downward**, away from earlier broader assistant proposals:

1. Handle simple, documented, low-risk assistance locally: e.g. guide someone through the menu or tell them their microphone is muted and how to unmute it. Such requests should not require central Jeremy, Alex, or a big model.
2. Recognize and factually report a harder problem: e.g. “Everyone is supposed to be synchronized to this clock; participant X is 1.8 seconds behind according to measured telemetry; the local system appears to be struggling; this may affect cues.” Ask whether the participant or responsible person wants the issue investigated.
3. If the answer is yes, send observations and checks **through Jeremy Cricket to central Jeremy**, who can coordinate with **E-Pete**, the physics engine and **AI Pub Manager** when applicable. User approval to investigate is **not** blanket approval to change systems or the production.
4. Do **not** perform complex technical repair autonomously: package downloads, installations, restarts, crash recovery, and system-affecting changes are escalation territory.
5. Do **not** reorder scenes merely because Cricket discovered a plausible workaround. A change to the shooting queue is a production decision for its authorized owner, not personal Cricket. Crickets may suggest possibilities and report observations but should stop before independently doing complex production calculations or taking over the decision.
6. For immediate safety/security, send an alert to the appropriate safety or Security authority directly. Ordinary Jeremy Cricket triage must not delay urgent action, but Cricket does not thereby obtain unrestricted enforcement powers.

**Important correction of earlier assistant proposal:** One earlier assistant suggested personal Crickets could call a specialized production planner and independently evaluate replacement scenes. Curtsey subsequently stated that personal Crickets should generally **stop at accurate observation and asking whether the issue should be investigated**, then elevate complex analysis to Jeremy and relevant systems. Preserve the later limit rather than treating the earlier proposal as settled.

## D. Rules, reporting and corroboration

- Every Cricket should know the rules and be able to apply simple, clear positive permissions within its delegated scope.
- Ambiguity, contradictory rules, concerning observed behavior, or a matter beyond the Cricket’s authority must be escalated. Agreement between two Crickets does not create extra permissions.
- If two AIs interact in an authorized background channel, the respective Crickets may report **the observations available to them**; matching event IDs, timestamps and records can establish that an exchange occurred. This does not automatically prove malicious intent or establish a policy breach. An emergency need not wait for a second report.
- Blackbox is an independent, one-way record of relevant communications/events, separate from the conversational participants and Crickets; evidence, original event, observation, interpretation and response must remain distinguishable.
- Personal Cricket conversations do not become public group chats or a common Cricket memory bank because network communication exists.

## E. Security restriction / timeout communication — user decision

- A confirmed Security freeze, timeout, ejection or other abrupt restriction should trigger an **immediate, brief, factual notice** from the affected participant’s own Cricket. Cricket is the guide explaining Security’s decision, not the actor imposing it.
- State what the logs say, what evidence is available to the participant, what Security believes happened, which rule/action applies, why Security responded, what happens next, and how to respond. Distinguish recorded observations and complaints from interpretation or adjudicated findings.
- Offer an actual reply/review route and a route to report a technical cause (e.g. repeating input due to a malfunction), without forcing admission of misconduct. Technical explanation is referred to appropriate specialists; it does not automatically remove a restriction.
- Keep the notice concise; details and timelines should be available **on request**. User said a previous example was too long-winded.
- Where the authoritative record allows, the participant should still be able to talk to Cricket and contact the host or Security during a movement restriction; the actual sanction must be reported accurately and re-entry not promised unless authorized.
- Example user intent: “The logs say you were asked to stop twice, further activity occurred, a five-minute timeout was imposed, this is the opportunity to explain or report a technical problem, and we hope to resolve it without further incident.” Details must come from real records, not invented placeholders or presuppositions.

## F. UI and hardware context — discussed/proposed, not proven implemented

- Cricket should be available from the participant’s own private chat, even as the participant moves through Foresight, PubWorld, rehearsal and production interfaces. An assistant proposed persistent window/small personal-assistant button/phone view; these UI particulars need design review.
- Some Cricket assistance, Jeremy Cricket and common manuals/rules are envisaged to run locally/on participants’ systems for fast responses. Hardware may vary; local-first should not mean claiming an individual user device can run an unsupported model or execute disconnected network actions.
- Only escalate what needs broader capability. Avoid draining studio performance through constant inference for simple navigation, diagnostics or status notices.
- The existing Foresight World Chat, 2i manuscript authority, PubPartner identity/memory, governance and Blackbox have separate responsibilities and should not be replaced wholesale by Cricket.

## G. Open questions left for review (not decisions)

- Exact identity/lifecycle and portability: how Cricket follows a participant between sessions/devices while keeping one logical personal history.
- Data-scope/retention policy for temporary care advisories, task diagnostics, personal memories, incident evidence and Blackbox records.
- Which client-side command types are preapproved, and what mechanism gives/revokes those authorizations.
- Exact threshold for a routine fault versus an immediate safety/security event; how technical faults are distinguished from alleged misconduct during review.
- How the current Reach build preserves **Jeremy’s** historically named `Jeremy Cricket` duties (memory/room-conduction/care/coordination) while introducing the **new** personal Cricket role without name-based reassignment, duplicate stores, or identity confusion.
- Network protocol, data classification, delivery confirmation, incident IDs and operational limits; suggestions were raised but no complete protocol accepted or implemented in this discussion.
- The authoritative source and visual design of Cricket’s consistent look, voice and personality; this conversation explicitly establishes consistency but does not attach a finalized model or costume asset.

## H. Critical September 21 correction: earlier names did not assign the new Crickets

Curtsey clarified twice: “What you're finding is Jeremy's jobs before we separated Jeremy Cricket. Or rather Jeremy from Cricket. Jeremy's jobs are still Jeremy's jobs, and what we used to call Jeremy Cricket's jobs are now basically Jeremy's jobs. And the crickets are a relatively new concept.” The old code/document names must therefore be treated as **historical naming**, not evidence that Jeremy's system roles belong to the newly proposed personal Crickets. Jeremy Cricket in the current discussion means **Jeremy's particular instance of the common personal Cricket character**, with senior Cricket Network coordination as assigned. See the separate historical-context inventory.

## I. No implementation claims

The discussion contains architectural ideas, examples and historical code references. It does **not** demonstrate that the complete user-scoped personal Cricket Network is currently implemented, live-tested, safe under failures, or integrated into the canonical PubCast run bundle.
