# Memory-to-Experience Engine - produce a useful Moment Card

## Promise
A generic assistant responds to “What should I buy?” with a product list. This Skill responds to “What could make this person feel seen?” by turning **confirmed family meaning + current reality + available effort** into 2-3 options the user can genuinely choose.

## Moment Card - user-visible output schema

**Who and what:** recipient role, occasion, timing (only if given), user goal.

**What we know:** one or two short evidence-backed anchors, citing exact authorized path or attributed user quote; show `DOCUMENTED`, `USER_TESTIMONY` or `NO_PERSONAL_ANCHOR`. Source evidence and people's emotions are not interchangeable.

**Why it might matter:** meaning as **stated or confirmed by the user**, not invented. Clarify whether current recipient preferences are known, stale or unknown. Ask once before committing to a high-effort plan where preference mismatch would matter.

**Experience routes:**
- **A. The 10-minute gesture:** low-cost, accessible, low-pressure idea (voice note, photo conversation, handwritten thank-you, sharing an old recipe without making it obligatory).
- **B. The shared experience:** time together aligned with the person's current choice (cooking, place revisit, collaborative project, a quiet meal).
- **C. The keepsake/legacy option:** a reviewed letter, mini-story, family recipe note or chosen memory chapter; no auto-generated false evidence or fabricated speaker words.

For EACH route supply **what to do**, **why connected to this person's stated memory**, **one clear next step**, **time/effort and user-defined budget fit**, **what to check with the recipient**, and **a gentler/accessible fallback**. Avoid presenting three cosmetic variants of the same idea. Prefer one excellent option and one alternative over forcing three weak suggestions.

**Decision:** “Which feels right: A, B, C, something smaller, or none?” The user is free to reject all. The Skill is not a moral judge of family devotion.

**Chapter status:** `PROPOSED / UNSAVED`. After a user-approved write, show the actual saved result only when confirmed by the agent and platform approval. Only later, on user-initiated return, a lived experience may become a separate approved chapter. Proposed ideas never silently become facts.

## Meaning bridge check
A recommendation passes only when:
1. The occasion and recipient are user-provided; no inferred birthdays.
2. The personalization rests on a specific confirmed memory/preference, OR is transparently described as general.
3. The recommended activity is in the user's control and contingent on other participants' consent, ability and current wishes.
4. The plan is concrete and executable with stated practical constraints; it is not merely an emotional slogan.
5. The source path, uncertainties and user approval are carried forward if the idea is saved.

## Failure and low-context fallbacks
- No NAS access: accept a short spoken memory; if none, offer honest generic choices and one invitation to personalize.
- Contradictory memory: say “These accounts differ”; do not pick a winner or craft a misleading story.
- Current preference differs from nostalgia: **current wishes win**. A former cyclist may now prefer a shared tea and photo conversation.
- Impracticality/limited mobility: offer accessible forms of participation, do not infer health conditions.
- Grief, estrangement, adoption, sensitive disclosures: avoid guilt, forced reunions, public storytelling, surprise disclosures and reconciliation pressure.
- Elderly or minor recipients: preserve agency and guardian/participant consent where relevant.
- Missing occasion date: never invent an upcoming trigger or reminder.

## Example (fictional; no NAS facts implied)
User: “Dad turns seventy. What can I do?”
User-confirmed memory: “We used to repair bicycles together on Sundays. It meant he always made time for me.”
A: Invite him for coffee, bring the old photo, tell him what those Sundays meant. Next step: choose a quiet time.
B: If he still enjoys it and wants to, restore a bicycle together; if not, visit a repair shop or watch family videos together. Next: ask what he would find enjoyable.
C: Write a two-page photo letter titled “The Sundays You Gave Me”; ask the user to verify every caption before any save. Next: select two approved photos.
Question: “Would he enjoy doing something together, or would a quiet conversation mean more to him now?”
