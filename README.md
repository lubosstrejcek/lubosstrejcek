# Hi there, I'm Lubos Strejcek 👋

## About Me

🔋 Interested in **energy monitoring**, **home automation**, and **IoT**
🏠 Building smart home solutions with open-source tools
📍 Czech Republic

---

## 🌟 Featured Project: Victron Energy Monitoring Stack

A complete Docker-based monitoring solution for Victron Energy systems.

Created during **Victron Energy Training Center Brno - Node-RED Training**.

### Architecture

```
┌─────────────┐      ┌─────────────┐      ┌─────────────┐      ┌─────────────┐
│  Ekrano GX  │─MQTT─▶│  Node-RED   │─────▶│  InfluxDB   │─────▶│   Grafana   │
│   (Victron) │      │  (Process)  │      │  (Store)    │      │ (Visualize) │
└─────────────┘      └─────────────┘      └─────────────┘      └─────────────┘
```

### Repositories

| Component | Description | Status |
|-----------|-------------|--------|
| [**victron-nodered**](https://github.com/lubosstrejcek/victron-nodered) | Node-RED flows for MQTT data collection | ✅ Ready |
| [**victron-influxdb**](https://github.com/lubosstrejcek/victron-influxdb) | InfluxDB 2.x time-series database | ✅ Ready |
| [**victron-grafana**](https://github.com/lubosstrejcek/victron-grafana) | Grafana dashboards with auto-provisioning | ✅ Ready |

### Quick Start

```bash
# Clone all three repos and run with docker compose
git clone https://github.com/lubosstrejcek/victron-influxdb && cd victron-influxdb && cp .env.example .env && docker compose up -d && cd ..
git clone https://github.com/lubosstrejcek/victron-nodered && cd victron-nodered && cp .env.example .env && docker compose up -d && cd ..
git clone https://github.com/lubosstrejcek/victron-grafana && cd victron-grafana && cp .env.example .env && docker compose up -d && cd ..
```

---

*Feel free to use these repositories for inspiration or as a starting point for your own Victron monitoring setup.*
