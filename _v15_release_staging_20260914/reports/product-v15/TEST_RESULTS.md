# V15 Test Results

## Focused baseline

Command:

```text
uv run pytest -q tests/test_wp07_foundation_assist.py tests/test_agent_mission_runtime.py
```

Result: `9 passed`.

## V15 focused suite

Command:

```text
uv run pytest -q tests/test_v15_copilot.py
```

Result: `5 passed`.

Coverage includes the intent matrix, hypothetical-vs-current routing, read-only What-If simulation, no Twin/Event mutation, explicit disruption Event creation, and honest fallback labeling.

## V14 convergence reference

Command:

```text
uv run pytest -q tests/test_v15_copilot.py tests/test_v14_grounded_adaptive_recovery.py
```

Result: `7 passed`.

## Broad backend regression

Command:

```text
uv run pytest -q
```

The process completed without a recorded failure. The cache contained 417 collected node IDs and `{}` for `lastfailed`. The first terminal polling wrapper stopped displaying progress at 54%, so the exact final pass/skip line is intentionally not reconstructed.

## Frontend and browser

- `npm run build`: passed; Vite generated the production PWA bundle and reported only the existing >500 kB chunk warning.
- Playwright: Fuzhou generic-city flow passed with honest unavailable evidence; sealed Tianjin stay selection followed by What-If submission passed with the UI badges/card visible and zero console errors.
- Screenshots: `output/playwright/v15-fuzhou-copilot.png`, `output/playwright/v15-tianjin-copilot-what-if.png`.
