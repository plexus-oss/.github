# Plexus

Telemetry for hardware teams sensor data in, one timeline, a UI you don't
have to build. [plexus.company](https://plexus.company)

This organization hosts the **open device-side code**: the pieces that run
inside your hardware and your ground system. The Plexus platform itself is
commercial and not distributed here.

---

### [plexus-python](https://github.com/plexus-oss/plexus-python) — Python SDK · Apache-2.0

Stream telemetry from any device in one line. Store-and-forward SQLite buffer
for intermittently connected hardware, WebSocket and HTTP transports, and
examples for CAN bus, MAVLink, MQTT, I2C sensors, and thermal cameras.

```bash
pip install plexus-python
```

```python
from plexus import Plexus

px = Plexus(api_key="YOUR_KEY", source_id="robot-01")
px.send("battery.voltage", 12.4)
```

### [openc3-cosmos-plexus](https://github.com/plexus-oss/openc3-cosmos-plexus) — COSMOS plugin · MIT

Tails decommutated telemetry out of [OpenC3 COSMOS](https://openc3.com) into
Plexus, and frames Plexus screens inside COSMOS. Installs into your existing
ground system.

---

Both are licensed so that code shipping inside your hardware carries no
strings. Issues and pull requests welcome on either.

Commercial platform, pricing, and self-hosted deployments:
[plexus.company](https://plexus.company) · info@plexus.company
