# Family Meaning Graph - evidence-grounded session context

## Purpose and runtime boundary
The Family Meaning Graph is **an explanatory reasoning scaffold reconstructed in the present conversation**, not a durable graph database, invisible background scanner, biometric identity system or independently executing service. Its purpose is to answer *what makes this occasion uniquely meaningful?* without pretending to read people's minds.

## Nodes
- `PERSON`: user-described role/name as volunteered; never identify from a face alone. A person not present is not automatically an authorized participant.
- `MOMENT`: user-described life event or evidence-linked event candidate; status `DOCUMENTED`, `USER_TESTIMONY`, `INFERRED`, `UNKNOWN` or `CONFLICTING`.
- `SOURCE`: exact selected, authorized NAS path/album/photo pointer actually returned, or `USER_TESTIMONY` with speaker attribution; each claim points back to source.
- `PREFERENCE`: direct quote or user-reported, date-stamped when available. Preferences can change. `CURRENT_PREFERENCE_UNKNOWN` is a useful state.
- `MEANING`: the **speaker's interpretation in their own words**; do not infer love, grief, reconciliation, regret or closeness from an image.
- `OCCASION`: occasion named by user, deadline/date if provided, practical constraints, consent and proposed audience.
- `EXPERIENCE`: prospective gesture, shared activity or keepsake; status `PROPOSED`; no claim of purchase or execution.

## Edges
- `PARTICIPATED_IN`, `RECALLS`, `DOCUMENTED_BY`, `MATTERS_TO`, `WISHES_TO_CONTINUE`, `INSPIRED_PROPOSAL`.
- Every edge has `evidence_label`, `source_pointer_or_user_quote`, `speaker`, `review_state`, optional `time_precision`, and explicit `share_scope` where known.
- Distinguish **observed evidence** (e.g., a bicycle appears in the photograph) from **user interpretation** (e.g., Dad made time every weekend). Keep human recollections as testimony, not file-proven facts.

## Minimal example (fictional)
- `S1`: authorized photograph shows an adult and child near a bicycle; exact date uncertain. `DOCUMENTED` only for visible objects and people, **not identity**.
- User confirms: “That was Dad and me. We repaired bikes on Sundays.” This is `USER_TESTIMONY`.
- User adds: “Those afternoons made me feel important to him.” This is the user's **meaning**.
- `O1`: Dad's seventieth birthday; user wants a quiet experience; budget low; recipient's current physical ability and interest unconfirmed.
- `E1`: restore an old bicycle together, **conditionally** if Dad would enjoy and can comfortably participate; alternative: look at the photograph and share the story over coffee.

## Graph assembly protocol
1. Obtain user intent, and only if requested ask for a narrowly scoped NAS source; no whole-library scan.
2. Create a source ledger from actual results and user-supplied statements; do not fabricate absent nodes.
3. Show a proposed meaning bridge as a question: “Was fixing bicycles something you enjoyed together?”
4. Ask the user to confirm/correct the bridge. If denied, remove it from the proposal; do not treat correction as resistance.
5. Derive experience ideas from **confirmed** meaning plus current practical constraints. Label unsupported relations as candidate questions, not facts.
6. Do not automatically store the graph. A new selected Moment Card or chapter may be saved as text **only** after user review and platform workflow approval, following SKILL.md Section 6.

## Boundaries
A shared folder is not blanket permission to disclose one relative's life to another. Do not infer health, family conflict, emotions, financial means, religion or other sensitive traits from images. Do not identify unknown people by facial recognition, infer a minor's preferences without asking, or surface secrets in a group celebration. Never claim a verified persistent graph, automatic cross-session retrieval, or background learning.
