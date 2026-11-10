# In-session memory and intention ledger - conceptual only

This is a structured **in-conversation** representation, not a permanent database, automated NAS graph or promised cross-session agent memory.

Record types:

- `PERSON`: only user-identified or independently sourced with appropriate permission; display scope
- `PLACE`: actual source(s), name and temporal precision
- `PERIOD`: coarse or exact date range, uncertainty and source
- `EVENT`: confirmed or tentative past/present occurrence; evidence and contradictions
- `CLAIM`: attributed proposition, evidence status, source and user review
- `CHAPTER`: story title, lens, review note, exact approved source IDs/paths
- `INTENTION`: a user's desired **future** experience, user-selected purpose lens, confirmed memory anchor, why the bridge matters **as stated by that user**, optional related chapter, `Life stage: UNWRITTEN`; this is not a factual event
- `OCCASION`: user-described celebration or everyday moment; intended person, time window, constraints and optional approved sources, not an inferred calendar or auto-reminder event
- `RELATIONSHIP_CONTEXT`: user-confirmed preference or personally told shared memory for a chosen recipient; transient unless separately reviewed and saved
- `CARE_IDEA`: suggested gift, gesture, shared celebration or ritual with a meaningful reason, `SUGGESTED` status and no executed action
- `RETURN_ACCOUNT`: later user account and optional new actual evidence for a previously unwritten chapter; never auto-attach to an intention without explicit review

Only connect records when evidence is real or a user confirms a proposed association. One new user fact may clarify multiple **already inspected authorized** records (in-session Memory Ripple); show matches for approval and do not touch original metadata. Never silently replace a person's contrary recollection.

A later session starts from the **exact previously saved text path the user selects**, read via authorized `ug-filesystem cat` if actually accessible. Otherwise ask for that text. No whole-NAS cross-session memory search or graph synchronization is assumed.

Use two separate states for future documents: `Life stage: UNWRITTEN|LIVED` vs `Record state: DRAFT|APPROVED_SAVED`. Only verified `save-text` completion changes the record state to `APPROVED_SAVED`. See [future_chapter.md](future_chapter.md) for writing behavior.
