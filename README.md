# Valheim Watch

Shared dashboard: https://bozhidardev.github.io/valheim-watch/

This is the public frontend for the Valheim server monitor. It reads saved reports
from the existing public status API; page visits never query the game server.
The collector continues running on Northflank. Credentials and collector source
are kept in their existing private deployment.

The dashboard preserves history, player counts, alerts while open, CSV export,
and the distinction between a Crossplay listing and confirmed game joinability.

## Development

Install Node.js 22+ and run `npm ci`, then `npm run dev`.
Build with `npm run build`. The base path is `/valheim-watch/`.

GitHub Pages publishes the `dist` artifact through the Pages workflow on pushes
to `main`. Free Pages hosting uses this public repository.
