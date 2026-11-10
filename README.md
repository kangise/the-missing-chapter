# The Missing Chapter

> **Don't just remember the moments that mattered. Make more of them.**

*The Missing Chapter* is a consent-first AI Skill for **AI-powered NAS agent platforms**. It helps families turn trusted memories into personal gestures, shared experiences, and new moments worth remembering.

## The problem

Busy families know the important dates, but often struggle to make someone feel truly *seen*. A NAS can hold thousands of archived photos, yet those photos record **what happened**, not **why it mattered**. As a result, a birthday gift turns generic, and a graduation celebrates the certificate but overlooks the journey.

Calendars recall dates. Photo apps surface images. Shopping assistants rank products. None of them connect a real memory to a meaningful action.

## The idea

```
TRUSTED MEMORY  →  HUMAN MEANING  →  PURPOSEFUL ACTION
```

Imagine a father turning seventy. Instead of "what should I buy?", the child shares an old bicycle photo and confirms a memory: *"He taught me to repair bikes every Sunday."* The Skill turns that confirmed meaning into a few feasible options, such as a coffee-and-photo conversation, restoring a bicycle together (if he wants to), or a short illustrated letter. The user chooses, adapts, and decides whether to save the result.

The same approach works for graduations, anniversaries, reunions, gratitude, or an ordinary Sunday.

## How it works

1. **Ask naturally**: "How can we celebrate Dad?" No forms and no mode labels.
2. **Give one remembered detail**, or approve a narrow NAS source (one album, one folder). A NAS is optional. The Skill also works with only the user's own story.
3. **At most two questions**: the Skill asks only what it truly needs.
4. **A Moment Card with three routes**: a small gesture, a shared experience, and a keepsake or ritual. Each shows its evidence, certainty, consent status, a low-effort alternative, and an optional way to preserve the moment.
5. **The user decides.** Plans stay `PROPOSED`, never `LIVED`.
6. **Optional follow-up.** After the real event, the user can tell the Skill what actually happened and save it as a new, separately approved chapter.

### Modes

| Mode | What it does |
| --- | --- |
| **Make a Moment Meaningful** | Everyday care and occasions: gifts, celebrations, thank-yous |
| **Discover My Past** | Source-linked memory clues, guided questions, a corrected story draft |
| **Capture This Moment** | Preserve a current event from new photos or testimony |
| **Write My Future** | A purposeful *Unwritten Chapter* rooted in a confirmed memory, never a forecast |
| **Return to a Chapter** | Revisit a saved chapter and write a new version after the event |

### Three in-session engines

- **Family Meaning Graph**: a temporary, auditable set of user-confirmed people, moments, preferences, and permissions. Links are *proposals* until the user confirms them. It is not a persistent database.
- **Memory-to-Experience Engine**: turns a confirmed memory into a **Moment Card** with concrete options a person can actually choose.
- **Family Memory Flywheel**: voluntary only. After a real event, the user's account becomes a new chapter that can inspire the next one.

## NAS capabilities used

The parent Skill only delegates to registered expert agents. Each expert selects and runs its own supported CLI actions.

| Expert agent | CLI | Actions | Purpose |
| --- | --- | --- | --- |
| `photo-agent` | `ug-photo` | `albums`, `search-picture`, `meta`, `vision-vlm` | Search a selected album and inspect returned photos |
| `file-agent` | `ug-filesystem` | `find`, `cat` | Find approved documents or read a prior chapter |
| `document-agent` | `ug-document` | `qa`, `extract` | Extract dates, places, and clues from approved files |
| `knowledge-agent` | `ug-knowledge` | `audio-transcription`, `save-text` | Transcribe one consented recording, or save approved text |

Checked against the platform capability catalog v2.0.0.

## Trust and privacy principles

- **Least-privilege access.** Exact user-approved album or folder only, with initial limits of 24 photos and 8 documents. No whole-NAS scans.
- **Evidence labels.** Every claim is marked `DOCUMENTED`, `USER_TESTIMONY`, `INFERRED`, `UNKNOWN`, `CONFLICTING`, or `PARTIAL_COVERAGE`. No emotional interpretation is presented as fact.
- **Two-step save.** The user approves the content, then the platform approves the workflow. The Skill only creates *new* files and never overwrites.
- **Honest failures.** If a save fails, the chapter stays an unsaved draft. Success is never claimed without completion evidence.
- **Recipient first.** The recipient's current preferences and consent outweigh nostalgia.

### What it deliberately does *not* do

No automatic reminders, purchases, guest messages, calendar events, media generation, durable knowledge graph, or device control. It does not predict the future, impersonate absent relatives, profile children, clone voices, or record a home in the background. Future ideas such as phone import, family displays, and time capsules are described only as concepts in [`references/ecosystem_vision.md`](references/ecosystem_vision.md), and nothing in the Skill claims to implement them.

## Repository layout

```
.
├── SKILL.md                      # The Skill: orchestration, modes, delegation, approvals
└── references/                   # Linked design references
    ├── everyday_care.md          # High-frequency occasion entry point
    ├── memory_to_experience.md   # Moment Card format
    ├── family_meaning_graph.md   # In-session graph semantics
    ├── family_flywheel.md        # Voluntary follow-up loop
    ├── future_chapter.md         # Unwritten Chapter design
    ├── moment_scenarios.md       # Birthday, graduation, anniversary playbooks
    ├── signature_demo.md         # Fictional two-minute demo
    ├── privacy_guardrails.md     # Consent and safety rules
    ├── evidence_policy.md        # Evidence labels
    ├── validation_cases.md       # Test cases
    └── ...                       # story format, memory record, disclosures, etc.
```

## Status

- Authored workflows, Moment Card format, graph semantics, occasion playbooks, consent controls, and error handling are complete as Markdown references.
- The platform's static check **passed**.
- **Not yet tested:** real NAS installation, runtime model routing, and cross-session persistence. Local model use is preferred when verified, and this Skill initiates no external service calls.

## Validation plan

- **Core A:** an authorized bicycle photo and a corrected recollection produce a meaningful birthday plan and an approved text save.
- **Core B:** a graduation photo plus family testimony yields an actionable celebration.
- **Edge:** denied album access or contradictory memories lead to transparent fallbacks, never invented facts or unauthorized writes.

## Disclosures

- AI drafting assistance: OpenAI ChatGPT. See [`references/disclosures.md`](references/disclosures.md).
- No bundled SDKs, binaries, third-party media, model weights, or real personal data. All family examples are fictional.
- The host NAS platform's components remain subject to its own terms and are not redistributed here.

## License

No open-source license has been granted yet. All rights are reserved by the author unless a license file is added.
