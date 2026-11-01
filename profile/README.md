# Make Things Happy!
The official GitHub home for the [makethingshappy.io](https://makethingshappy.io) platform.  
High-quality hardware modules and software for seamless IoT/IIoT integration.

---

## 📋 Contents

- [🔧 Our Ecosystem](#-our-ecosystem)
- [📊 Software Compatibility](#software-compatibility)
  - [Carrier Boards](#carrier-boards)
  - [IoTextra — Software Compatibility](#iotextra--software-compatibility)
  - [IoTextra — Node-RED Compatibility](#iotextra--node-red-compatibility)
  - [IoTextra — Tasmota Compatibility](#iotextra--tasmota-compatibility)
  - [IoTextra — ESPHome Compatibility](#iotextra--esphome-compatibility)
- [📰 Publications](#-publications)

---

## 🔧 Our Ecosystem

**Make Things Happy** builds a unified, modular platform for IoT and industrial automation:

| Layer | Product | Description |
|---|---|---|
| **Software** | [IoTflow](https://github.com/makethingshappy/IoTflow) | Workflow orchestration platform. Node-RED + MQTT + MicroPython |
| **Controllers** | [IoTsmart](https://github.com/makethingshappy/IoTsmart) | SoM boards: ESP32-S3, RP2040, RP2350A |
| **Carrier Boards** | [IoTbase](https://github.com/makethingshappy/IoTbase) | Professional carrier boards for Arduino Nano, Raspberry Pi Pico, Adafruit Feather |
| **Carrier Boards** | [IoTbase-RPi](https://github.com/makethingshappy/IoTbase-RPi-Test) | Carrier board for Raspberry Pi (SBC) |
| **I/O Modules** | [IoTextra-Digital](https://github.com/makethingshappy/IoTextra-Digital) | Isolated digital I/O modules and relays |
| **I/O Modules** | [IoTextra-Analog](https://github.com/makethingshappy/IoTextra-Analog) | High-precision analog I/O modules |
| **I/O Modules** | [IoTextra-Combo](https://github.com/makethingshappy/IoTextra-Combo) | Hybrid analog & digital I/O modules |
| **Smart Home** | [IoThome](https://github.com/makethingshappy/IoThome) | Standalone Tasmota ecosystem for smart home |
| **Smart Home** | [MTH for ESPHome](https://github.com/makethingshappy/MTH-for-ESPHome) | ESPHome support for makethingshappy.io modules: ready-to-flash configs and setup guide |
| **Adapters** | [Shields](https://github.com/makethingshappy/Shields) | Adapters connecting Arduino, Feather, Pico, Teensy to mikroBUS |

---

## <a name="software-compatibility"></a>📊 Software Compatibility

IoTextra modules work with three software platforms:

- **[IoTflow](https://github.com/makethingshappy/IoTflow)** — Node-RED, MQTT and Blynk
- **[IoThome](https://github.com/makethingshappy/IoThome)** — Tasmota templates and Berry drivers
- **[MTH for ESPHome](https://github.com/makethingshappy/MTH-for-ESPHome)** — ESPHome configs ([setup guide](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Documentation/Setup.md))

The tables below show what is available for each carrier board and IoTextra module.

### Carrier Boards

<!-- CARRIER_COMPATIBILITY_START -->
# Carrier Board Software Compatibility

| Carrier Board | host-map | IoTflow (Node-RED) | MTH for Tasmota (formerly IoThome) | MTH for ESPHome |
|---|:---:|:---:|:---:|:---:|
| IoTbase PICO v.3.05 + RP2040 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.05/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — | — |
| IoTbase PICO v.3.05 + RP2350 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.05/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — | — |
| IoTbase PICO v.3.06 + Waveshare ESP32-S3-Pico | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.06/host-map.yaml) | 🔶 Coming Soon | 🔶 Coming Soon | 🔲 Planned |
| IoTbase PICO v.3.06 + Waveshare ESP32-C6-Pico | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.06/host-map.yaml) | 🔶 Coming Soon | 🔶 Coming Soon | 🔲 Planned |
| IoTbase PICO v.3.06 + RP2040 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.06/host-map.yaml) | 🔶 Coming Soon | — | — |
| IoTbase PICO v.3.06 + RP2350 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/PICO/v.3.06/host-map.yaml) | 🔶 Coming Soon | — | — |
| IoTbase NANO v.3.06 + Waveshare ESP32-S3-NANO | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTbase/blob/main/NANO/v.3.06/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/Documentation/Setup.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Documentation/Setup.md) |
| IoTbase Feather + Adafruit ESP32-C6 Feather | — | 🔶 Coming Soon | 🔶 Coming Soon | 🔲 Planned |
| IoTbase Feather + FeatherS3[D] ESP32-S3 | — | 🔲 Planned | 🔲 Planned | 🔲 Planned |
| IoTsmart RP2040 v.1.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/RP2040/v.1.02/host-map.yaml) | — | — | — |
| IoTsmart RP2350A v.1.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/RP2350A/v.1.02/host-map.yaml) | — | — | — |
| IoTsmart RP2350A v.2.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/RP2350A/v.2.02/host-map.yaml) | — | — | — |
| IoTsmart ESP32-S3 v.1.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/ESP32-S3/v.1.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/Documentation/Setup.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Documentation/Setup.md) |
| IoTsmart ESP32-S3 v.2.01 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/ESP32-S3/v.2.01/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/Documentation/Setup.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Documentation/Setup.md) |
| IoTsmart XIAO v.1.02 + XIAO RP2350 | — | — | — | — |
| IoTsmart XIAO v.1.02 + XIAO ESP32-S3 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/XIAO/v.1.02/host-map.yaml) | 🔶 Coming Soon | 🔶 Coming Soon | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Documentation/Setup.md) |
| IoTsmart XIAO v.1.02 + XIAO ESP32-C5 | — | 🔲 Planned | 🔲 Planned | 🔲 Planned |
| IoTsmart XIAO v.1.02 + XIAO ESP32-C6 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/IoTsmart/blob/main/XIAO/v.1.02/host-map.yaml) | 🔲 Planned | 🔲 Planned | 🔲 Planned |

**Legend:**
- [![Open](https://img.shields.io/badge/Open-green)]() — available, click to open
- — — not applicable
- 🔶 — Coming Soon
- 🔲 — Planned

<!-- CARRIER_COMPATIBILITY_END -->

### <a name="iotextra--software-compatibility"></a>IoTextra — Software Compatibility

<!-- IOTEXTRA_SOFTWARE_COMPATIBILITY_START -->
# IoTextra Software Compatibility

| IoTextra Module | host-map | IoTflow (Node-RED) | IoTflow (Blynk) | MTH for Tasmota (formerly IoThome) | MTH for ESPHome |
|---|:---:|:---:|:---:|:---:|:---:|
| Input v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Input/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| Relay v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Relay/v.3.02/host-map.yaml) | 🔶 Coming Soon | 🔶 Coming Soon | 🔶 Coming Soon | 🔶 Coming Soon |
| Relay2 v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Relay2/v3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| SSR Small v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/SSR%20Small/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| MOSFET2 v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/MOSFET2/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| Quadro | — | 🔲 | 🔲 | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔲 |
| Octal v.3.04 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Octal/v.3.04/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| Octal2 v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Octal2/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/README.md) |
| Octal3 v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Octal3/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔲 |
| Octal4 v.3.02 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-digital/blob/main/Octal4/v.3.02/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔶 |
| Analog v.3.12 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-analog/blob/main/Analog/v.3.12/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔶 |
| Analog2 | — | 🔲 | 🔲 | 🔲 | 🔲 |
| Analog3 v.3.11 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-analog/blob/main/Analog3/v.3.11/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔲 |
| Combo v.3.03 / v.3.04 | [![yaml](https://img.shields.io/badge/yaml-blue)](https://github.com/makethingshappy/iotextra-combo/blob/main/Combo/v.3.03_and_v.3.04/host-map.yaml) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/README.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/README.md) | 🔶 |
| Combo2 | — | 🔲 | 🔲 | 🔲 | 🔲 |

**Legend:**
- [![Open](https://img.shields.io/badge/Open-green)]() — available, click to open
- [![yaml](https://img.shields.io/badge/yaml-blue)]() — module host-map (pin and I2C map), click to open
- — — not applicable / not available
- 🔶 — Coming Soon
- 🔲 — Planned

<!-- IOTEXTRA_SOFTWARE_COMPATIBILITY_END -->

### <a name="iotextra--node-red-compatibility"></a>IoTextra — Node-RED Compatibility

<!-- IOTEXTRA_NODERED_COMPATIBILITY_START -->
# IoTextra Node-RED Compatibility

| IoTextra Module | Node-RED | Blynk |
|---|:---:|:---:|
| Input | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/input_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/input_board_flow_with_blynk.json) |
| Relay | 🔶 Coming Soon | 🔶 Coming Soon |
| Relay2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/relay2_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/relay2_board_flow_with_blynk.json) |
| SSR Small | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow_with_blynk.json) |
| MOSFET2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow_with_blynk.json) |
| Quadro | 🔲 | 🔲 |
| Octal | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow_with_blynk.json) |
| Octal2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow_with_blynk.json) |
| Octal3 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal3_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal3_board_flow_with_blynk.json) |
| Octal4 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow_with_blynk.json) |
| Analog | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/analog_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/analog_board_flow_with_blynk.json) |
| Analog2 | 🔲 | 🔲 |
| Analog3 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/analog_3_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/analog_3_board_flow_with_blynk.json) |
| Combo | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/combo_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/combo_board_flow_with_blynk.json) |
| Combo2 | 🔲 | 🔲 |

**Legend:**
- [![Example](https://img.shields.io/badge/Example-yellowgreen)]() — available, click to open
- 🔶 — Coming Soon
- 🔲 — Planned

<!-- IOTEXTRA_NODERED_COMPATIBILITY_END -->

### <a name="iotextra--tasmota-compatibility"></a>IoTextra — Tasmota Compatibility

<!-- IOTEXTRA_TASMOTA_COMPATIBILITY_START -->
# IoTextra Tasmota Compatibility
| IoTextra Module | IoTsmart ESP32-S3 | IoTsmart XIAO + XIAO ESP32-S3 | IoTbase PICO + Waveshare ESP32-S3-Pico | IoTbase NANO + Waveshare ESP32-S3-NANO | IoTbase Feather + Adafruit ESP32-C6 Feather |
|---|:---:|:---:|:---:|:---:|:---:|
| Input | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-input) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-input) | 🔶 |
| Relay | 🔶 Coming Soon | 🔶 Coming Soon | 🔶 Coming Soon | 🔶 Coming Soon | 🔶 Coming Soon |
| Relay2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-relay2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-relay2) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-relay2) |
| SSR Small | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-ssr-small) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-ssr-small) | 🔶 |
| MOSFET2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-mosfet2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-mosfet2) | 🔶 |
| Quadro | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-quadro) | 🔲 | 🔲 | 🔲 | 🔲 |
| Octal | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-octal) |
| Octal2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal2) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-octal2) |
| Octal3 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal3) | 🔲 | 🔲 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal3) | 🔲 |
| Octal4 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal4) | 🔲 | 🔲 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal4) | 🔲 |
| Analog | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-analog) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-analog) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-analog) |
| Analog2 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Analog3 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-analog3) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-analog3) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-analog3) |
| Combo | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-combo) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-combo) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-combo) |
| Combo2 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |

**Legend:**
- [![Template](https://img.shields.io/badge/Template-green)]() — available, click to open
- 🔶 — Coming Soon
- 🔲 — Planned

<!-- IOTEXTRA_TASMOTA_COMPATIBILITY_END -->

### <a name="iotextra--esphome-compatibility"></a>IoTextra — ESPHome Compatibility

<!-- IOTEXTRA_ESPHOME_COMPATIBILITY_START -->
# IoTextra ESPHome Compatibility
| IoTextra Module | IoTsmart ESP32-S3 | IoTsmart XIAO + XIAO ESP32-S3 | IoTbase PICO + Waveshare ESP32-S3-Pico | IoTbase NANO + Waveshare ESP32-S3-NANO | IoTbase Feather + Adafruit ESP32-C6 Feather |
|---|:---:|:---:|:---:|:---:|:---:|
| Input | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-input-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-input-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-input-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Relay | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Relay2 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-relay2-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-relay2-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-relay2-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| SSR Small | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-ssr-small-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-ssr-small-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-ssr-small-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| MOSFET2 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-mosfet2-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-mosfet2-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-mosfet2-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Quadro | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Octal | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-octal-v3-04-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-octal-v3-04-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-octal-v3-04-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Octal2 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-octal2-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-octal2-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [![Config](https://img.shields.io/badge/Config-green)](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-octal2-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Octal3 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Octal4 | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-octal4-v3-02-iotsmart-esp32s3-v2-01-gpio.yaml) | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-octal4-v3-02-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-octal4-v3-02-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Analog | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-analog-v3-12-iotsmart-esp32s3-v2-01-i2c.yaml) | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-analog-v3-12-iotsmart-xiao-v1-02-i2c.yaml) | 🔲 | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-analog-v3-12-iotbase-nano-v3-06-i2c.yaml) | 🔲 |
| Analog2 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Analog3 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
| Combo | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_ESP32-S3/iotextra-combo-v3-04-iotsmart-esp32s3-v2-01-gpio.yaml) | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTsmart_XIAO_XIAO-ESP32-S3/iotextra-combo-v3-04-iotsmart-xiao-v1-02-gpio.yaml) | 🔲 | [🔶](https://github.com/makethingshappy/MTH-for-ESPHome/blob/main/Configs/IoTbase_NANO_Waveshare-ESP32-S3-NANO/iotextra-combo-v3-04-iotbase-nano-v3-06-gpio.yaml) | 🔲 |
| Combo2 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |

**Legend:**
- [![Config](https://img.shields.io/badge/Config-green)]() — config available and verified on hardware, click to open
- 🔶 — config published, not yet verified on hardware
- 🔲 — Planned

<!-- IOTEXTRA_ESPHOME_COMPATIBILITY_END -->

---

## 📰 Publications

Articles and press about our projects — [view full list](PUBLICATIONS.md)

---

*© Make Things Happy — makethingshappy.io*
