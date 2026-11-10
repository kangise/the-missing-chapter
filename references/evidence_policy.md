# Evidence and temporal-grounding policy

- `DOCUMENTED`: a narrow factual claim is supported by a real, authorized NAS source; include real path/ID and date precision
- `USER_TESTIMONY`: speaker-attributed report of an event, feeling or relationship; not independently verified
- `USER_INTENT`: a first-person wish, hope, plan or letter about a future experience; **never evidence that it occurred**
- `INFERRED`: tentative association with explanation; ask for confirmation, no invented identification
- `UNKNOWN`: not established within selected scope, including future outcomes
- `CONFLICTING`: source and testimony disagree, so retain both without forced adjudication
- `PARTIAL_COVERAGE`: only a subset of source data was inspected or an authorized tool did not complete

Represent claims conceptually as `{claim; source_id/path or user statement; time orientation (past/present/future); evidence_label; date precision; review status}`. Do not instantiate a hidden persistent store.

Memory Detective: propose only **source-anchored questions** from actual limited results, not grand conclusions or identity linkage. Memory Ripple: one confirmed answer may explain *already authorized evidence* and should show proposed matches. No automated life-event detection, risk scoring, face identity resolution, regret judgments, future prediction, fabricated photos or fake deceased-person messages.

When evidence is weak, give a gentle question or a sparse outline. When future data is entirely user-authored, say `User-authored; no NAS evidence consulted`.
