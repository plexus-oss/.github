# Plexus — Ingest. Observe. Control.

HardwareOps platform guide for using Plexus.

---

### [plexus-python](https://github.com/plexus-oss/plexus-python) — Python SDK

Stream sensor data, CAN bus, MAVLink, cameras, and MQTT from any device.

```python
from plexus import Plexus

px = Plexus()
px.send("engine.rpm", 3450, tags={"unit": "A"})
```

```bash
pip install plexus-agent
```

---

### [plexus-c](https://github.com/plexus-oss/plexus-c) — Embedded C Library

Send telemetry from ESP32, STM32, and Arduino in ~1.5 KB RAM. Zero dependencies.

```c
plexus_client_t* px = plexus_init("plx_key", "esp32-001");
plexus_send(px, "temperature", 72.5);
plexus_flush(px);
```

---

### [plexus-ui](https://github.com/plexus-oss/ui) — GPU-Accelerated Charts

WebGPU/WebGL2 React components — 100k+ data points at 60fps.

```bash
npx plexusui init
npx plexusui add line-chart
```

---

[plexus.company](https://plexus.company) · [Documentation](https://docs.plexus.company) · [Discord](https://discord.gg/plexus)
