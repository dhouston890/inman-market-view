# Inman Market View — data + dashboard

Auto-published GitHub Pages site for Inman's local housing tools.

- **Housing dashboard:** https://dhouston890.github.io/inman-market-view/housing-dashboard/
- `dashboard_data/` — the sharded JSON / TopoJSON data cube the dashboard loads.
- `housing-dashboard/` — the static dashboard (`index.html` + assets).

Published automatically by `scheduled_refresh.sh` (weekly, Thursday afternoons)
from the Inman dashboard pipeline. The repo is kept at a single ever-green
commit (amend + force-push) so the cube never bloats git history — there is no
meaningful history to preserve since the cube is fully regenerable.
