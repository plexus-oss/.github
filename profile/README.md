# Plexus

Plexus is storage and dashboards for hardware teams: stream data from drones,
robots and IoT devices into Plexus Time Series, or connect the database you
already run, and get live dashboards and alerts. [plexus.company](https://plexus.company)

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

---

It is licensed so that code shipping inside your hardware carries no
strings. Issues and pull requests welcome.

Commercial platform, pricing, and self-hosted deployments:
[plexus.company](https://plexus.company) · info@plexus.company
