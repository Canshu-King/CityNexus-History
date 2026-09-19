# V15 Gate Matrix

| Gate | Result | Evidence |
|---|---|---|
| Package guidance read in order | PASS | `README_FIRST.md`, `CODEX_V15_OVERNIGHT_TASK_PROMPT.md`, policy/map/acceptance docs |
| Initial repository baseline | PASS | One `git status --short`; dirty worktree preserved |
| Existing focused baseline | PASS | 9 tests passed |
| Explicit semantic intents | PASS | `tests/test_v15_copilot.py` matrix |
| DeepSeek structured interpretation path | PASS | Existing Responses client + JSON schema boundary; live key unavailable and not claimed |
| Ordinary text does not fabricate Events | PASS | Preference, explanation, discovery, and hypothetical API tests |
| Current disruption Event path | PASS | Only `DISRUPTION_REPORT` creates `user-copilot` / `USER_REPORTED` Event |
| Read-only What-If invariants | PASS | No Event or JourneyTwin row change in focused API test |
| V14 recovery reference | PASS | `test_v14_grounded_adaptive_recovery.py` passed in convergence set |
| Broad backend regression | PASS* | Process completed with empty `.pytest_cache/v/cache/lastfailed`; 417 collected node IDs. Exact terminal summary was not retained by the first polling wrapper |
| Frontend production build | PASS | `npm run build` / Vite; existing chunk-size warning only |
| Generic-city browser flow | PASS | Fuzhou setup → City Discovery → Copilot; honest no-plan evidence |
| Sealed Tianjin browser What-If | PASS | Stay selection → AI desk → What-If card; console errors 0 |
| Secrets in source/artifact | PASS | No key added; release staging excludes env/key files |
| Fresh-extract release gate | PENDING AT REPORT AUTHORING | Executed after this report and package are created; final status is recorded in the release handoff |
