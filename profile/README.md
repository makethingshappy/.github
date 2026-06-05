# Make Things Happy!
The official GitHub home for the [makethingshappy.io](https://makethingshappy.io) platform.  
High-quality hardware modules and software for seamless IoT/IIoT integration.

---

## 📋 Contents

- [🔧 Our Ecosystem](#-our-ecosystem)
- [📊 Software Compatibility](#software-compatibility)
  - [Carrier Boards](#carrier-boards)
  - [IoTextra — Node-RED Compatibility](#iotextra--node-red-compatibility)
  - [IoTextra — Tasmota Compatibility](#iotextra--tasmota-compatibility)
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
| **I/O Modules** | [IoTextra-Digital](https://github.com/makethingshappy/IoTextra-Digital) | Isolated digital I/O modules with relays |
| **I/O Modules** | [IoTextra-Analog](https://github.com/makethingshappy/IoTextra-Analog) | High-precision analog I/O modules |
| **I/O Modules** | [IoTextra-Combo](https://github.com/makethingshappy/IoTextra-Combo) | Hybrid analog & digital I/O modules |
| **Smart Home** | [IoThome](https://github.com/makethingshappy/IoThome) | Standalone Tasmota ecosystem for smart home |
| **Adapters** | [Shields](https://github.com/makethingshappy/Shields) | Adapters connecting Arduino, Feather, Pico, Teensy to mikroBUS |

---

## <a name="software-compatibility"></a>📊 Software Compatibility

### Carrier Boards

<!-- CARRIER_COMPATIBILITY_START -->
# Carrier Board Software Compatibility

| Carrier Board | IoTflow (Node-RED) | IoThome (Tasmota) |
|---|:---:|:---:|
| IoTbase PICO + Waveshare ESP32-S3-Pico | 🔶 Coming Soon | 🔶 Coming Soon |
| IoTbase PICO + Waveshare ESP32-C6-Pico | 🔶 Coming Soon | 🔶 Coming Soon |
| IoTbase PICO + RP2040 | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — |
| IoTbase PICO + RP2350 | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — |
| IoTbase NANO + Waveshare ESP32-S3-NANO | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/Documentation/Setup.md) |
| IoTbase Feather + Adafruit ESP32-C6 Feather | 🔶 Coming Soon | 🔶 Coming Soon |
| IoTbase Feather + FeatherS3[D] ESP32-S3 | 🔲 Planned | 🔲 Planned |
| IoTsmart RP2040 | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — |
| IoTsmart RP2350A | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | — |
| IoTsmart ESP32-S3 | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoTflow/blob/main/Documentation/SETUP.md) | [![Open](https://img.shields.io/badge/Open-green)](https://github.com/makethingshappy/IoThome/blob/main/Documentation/Setup.md) |
| IoTsmart XIAO + XIAO RP2350 | 🔶 Coming Soon | — |
| IoTsmart XIAO + XIAO ESP32-S3 | 🔶 Coming Soon | 🔶 Coming Soon |
| IoTsmart XIAO + XIAO ESP32-C5 | 🔲 Planned | 🔲 Planned |
| IoTsmart XIAO + XIAO ESP32-C6 | 🔲 Planned | 🔲 Planned |

**Legend:**
- [![Open](https://img.shields.io/badge/Open-green)]() — available, click to open
- — — not applicable
- 🔶 — Coming Soon
- 🔲 — Planned

<!-- CARRIER_COMPATIBILITY_END -->

### <a name="iotextra--node-red-compatibility"></a>IoTextra — Node-RED Compatibility

<!-- IOTEXTRA_NODERED_COMPATIBILITY_START -->
# IoTextra Node-RED Compatibility

| IoTextra Module | Node-RED | Blynk |
|---|:---:|:---:|
| Input | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/input_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/input_board_flow_with_blynk.json) |
| Relay2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/relay2_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/relay2_board_flow_with_blynk.json) |
| SSR Small | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow_with_blynk.json) |
| MOSFET2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/output_board_flow_with_blynk.json) |
| Quadro | 🔲 | 🔲 |
| Octal | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow_with_blynk.json) |
| Octal2 | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow.json) | [![Example](https://img.shields.io/badge/Example-yellowgreen)](https://github.com/makethingshappy/IoTflow/blob/main/Node-RED%20Examples/octal_board_flow_with_blynk.json) |
| Octal3 | 🔲 | 🔲 |
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
| Relay2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-relay2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-relay2) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-relay2) |
| SSR Small | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-ssr-small) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-ssr-small) | 🔶 |
| MOSFET2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-mosfet2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-mosfet2) | 🔶 |
| Quadro | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-quadro) | 🔲 | 🔲 | 🔲 | 🔲 |
| Octal | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-octal) |
| Octal2 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTsmart_ESP32-S3.md#iotextra-octal2) | 🔶 | 🔶 | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Nano.md#iotextra-octal2) | [![Template](https://img.shields.io/badge/Template-green)](https://github.com/makethingshappy/IoThome/blob/main/Tasmota_Templates/IoTbase_Feather.md#iotextra-octal2) |
| Octal3 | 🔲 | 🔲 | 🔲 | 🔲 | 🔲 |
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

---

## 📰 Publications

Articles and press about our projects — [view full list](PUBLICATIONS.md)

---

*© Make Things Happy — makethingshappy.io*
