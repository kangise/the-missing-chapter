# Make a Moment Meaningful - high-frequency care and celebration design

## The human promise

People do not need another countdown calendar or a longer list of products. They need help remembering what makes someone feel seen, then turning that knowledge into a small, thoughtful choice. Family history is not a substitute for asking the person what they want today. This workflow works for a ten-minute gesture as well as a graduation ceremony, without implying uninterrupted monitoring of anyone's life.

**Core pattern:** A real occasion or human need -> a freely supplied / authorized memory -> what it means to the user -> two or three actionable options -> user choice and correction -> optionally an approved text plan -> a later user-initiated recollection of what actually happened.

## Common natural-language entry points

- "Mom's birthday is next week; what could I do that feels personal?"
- "Our daughter is graduating; how do we celebrate the journey rather than just the ceremony?"
- "Grandpa is visiting; I'd love to make an ordinary Sunday special."
- "I never thanked my teacher properly. What is a respectful gesture?"
- "My partner used to love that old family recipe. Can we create a new tradition?"
- "I have ten minutes. What small thing could make someone in my family feel appreciated?"
- "We missed a trip years ago. What new chapter could we choose together?"

## Fast interaction, not a mandatory intake

1. **Start with the request.** Identify occasion, approximate timing, intended recipient and outcome *only from what user actually said*. No automatic date or calendar lookup is supported. Do not ask for the user's whole family history.
2. **One small human question, only if useful.** "What's one little thing she loves, or a moment you both still remember?" Ask one second practical question only when genuinely needed (budget, abilities, ages, guest limits, or preference for a quiet/private vs public celebration). Accept "I don't know" and move on.
3. **Consent-first memory enrichment, optional.** If user wants to enrich the idea from NAS media, request a specifically selected authorized album/path or exact prior chapter. Then use root Skill's registered expert delegations. If no valid scope, do not search. No guest photos or named-person inference without permission.
4. **Meaning check.** Keep separate: `CONFIRMED_PREFERENCE` (user says); `USER_TESTIMONY` (their recollection); `DOCUMENTED` (supported by selected files); `SUGGESTED_IDEA` (AI option); `UNKNOWN` (not known). A birthday date is not evidence of what gift the recipient wants. If personal grounding is absent, say so.
5. **Offer 2-3 varied paths.** One small accessible gesture, one shared experience, and optionally one keepsake or ongoing ritual. For each include "Why this might fit" (and exactly what evidence supports it), "What it could look like", "A simpler way", "Ask or confirm before involving others", and "A memory worth preserving afterwards". User may request one path only or reject them all.
6. **Only with explicit user request**, turn a chosen idea into an editable **Occasion Chapter** with `Life stage: PLANNED`, not `LIVED`. Never claim a gift is purchased, event booked, message sent or family delighted. Review exact wording, privacy, filename and destination; require workflow approval for `ug-knowledge save-text`. No write if declined.
7. **After the event, only on return**, user says what actually occurred. Separate reality from original hopes and optionally draft a new approved `LIVED` memory chapter. No silent proactive follow-up or auto-scanning.

## Scenario A - a birthday that knows the person

Fictional demonstration. The user recalls that their mother always spoke fondly of making dumplings with her father. With no assumption that she wants to revisit it now, propose: (1) a short handwritten card mentioning that story; (2) an optional family cooking afternoon where *she* chooses the recipe and people; (3) a tiny recipe keepsake made from user-authorized materials. Ask whether it would feel comforting and welcome. No product purchase, reservation, guest contact or media output is implied.

## Scenario B - graduation as a bridge across time

The user explicitly selects a first-school-day photo and says their child once feared entering the classroom. Ask how the graduate wants to celebrate today. Offer an intimate first-day/to-graduation photo pairing plus parental letter, a small gathering with voluntary voice memories, or a chosen new shared experience. Do not infer emotions from the photo, publish an image, identify a child, or speak as the graduate. Narrate what the family *says*, not what the AI imagines happened.

## Scenario C - the ordinary Tuesday

An adult child asks how to thank a parent who quietly helps with childcare. No NAS reading is needed. Suggest a specific sincere voice note, taking over a disliked household task for an evening, or reserving an unhurried hour together if welcome. Avoid commercial pressure and guilt. A tiny act of care can count as a new chapter.

## Scenario D - a missed moment becomes a future chapter

A user recalls never taking a promised road trip. First ask whether they still *want* to explore it. Offer a nearby half-day variation if travel is difficult, or a different experience carrying the same feeling of adventure. Do not prescribe reconciliation, claim the missed trip harmed a relationship or require the original participants to join. If the user chooses a new plan, use `UNWRITTEN` and [future_chapter.md](future_chapter.md).

## Relevance without intrusion

- **Frequent access ≠ frequent notifications.** The current Skill is invoked on demand. Birthday reminders, opt-in calendar integrations, phone import, voice capture, room displays and family-event triggers are product roadmap items, not cataloged current actions.
- **Personal without invasive.** Prefer a meaningful memory explicitly offered by the user over unsolicited analysis of a household member, bystander, minor or guest.
- **Helpful without monetizing affection.** A free experience or sincere words can be more appropriate than a costly present. Honor user budget, accessibility, grief and relationship boundaries.
- **Respect different perspectives.** In a family celebration, the recipient may remember an event differently. Do not merge conflicting recollections or publicly display sensitive details without each person's consent.
