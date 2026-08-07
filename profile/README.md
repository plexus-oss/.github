# Plexus

Operations frontend for hardware fleets — connect any device or existing
telemetry store, get dashboards, instruments, and alerts that engineers
actually want to look at.

---

### [plexus](https://github.com/plexus-oss/plexus) — The platform

The whole thing: ingest gateway, ClickHouse storage, dashboards, alerts, read
API. Source-available under the Elastic License 2.0 — every feature is in the
repo; enterprise features unlock with an offline license key. Free for a
single team with no caps and **no phone-home**.

Self-host it in one command:

```bash
curl -fsSL https://plexus.company/install.sh | bash
```

---

### [plexus-python](https://github.com/plexus-oss/plexus-python) — Python SDK · Apache-2.0

Stream telemetry from any device — sensors, CAN bus, MAVLink, cameras, MQTT.

```bash
pip install plexus-python
```

```python
from plexus import Plexus

px = Plexus()
px.send("engine.rpm", 3450, tags={"unit": "A"})
```

---

### [plexus-typescript](https://github.com/plexus-oss/plexus-typescript) — TypeScript SDK · Apache-2.0

Node, browser, and edge runtimes — plus a drop-in ingest proxy for Next.js,
Remix, Hono, Bun, and Deno.

```bash
npm install plexus-typescript
```

```ts
import { Plexus } from "plexus-typescript";

const px = new Plexus({ sourceId: "relay-7" });
await px.send("engine_rpm", 3450, { tags: { unit: "A" } });
```

---

[plexus.company](https://plexus.company) · [docs.plexus.company](https://docs.plexus.company)
