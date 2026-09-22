<picture>
  <img alt="Hanyu Feng — Desktop software and device connectivity" src="https://raw.githubusercontent.com/vonpanda/vonpanda/main/assets/header.svg" width="100%">
</picture>

# 冯汉昱 · Hanyu Feng

**Desktop Software & Device Connectivity · 桌面软件与设备通信**  
`C++` `Qt / PyQt` `Python` `BLE` `Embedded Systems`

[English](#english) · [简体中文](#简体中文)

## English

I build software that connects computers and devices, from data acquisition and communication protocols to desktop monitoring and debugging tools. My background includes GPU virtualization development and embedded integration.

### What I work on

- **Desktop applications** — Qt / PyQt interfaces, device status monitoring, Windows device input handling, and cross-platform packaging.
- **Device connectivity** — Serial communication, BLE GATT / HID, MODBUS RTU, sensor data acquisition, and hardware–software integration.
- **Engineering tools** — Python automation, MCP integrations, and checks between schematic connections and firmware pin assignments.

### Current focus

Connecting device and firmware workflows with AI agent tools: structured hardware context through MCP, Python SDK integration, and explicit handling of uncertain results. I am exploring typed decision models for routing and operational triage; I have not yet benchmarked Jev on device data.

### Open-source contributions

- **TypeSafe Python SDK — HTTP/2 documentation:** prepared sync/async client examples with concurrent-request lifecycle checks. [Patch](https://github.com/typesafe-ai/typesafe-sdk-python/compare/main...vonpanda:typesafe-sdk-python:docs/http2-client-examples) · [Upstream discussion](https://github.com/typesafe-ai/typesafe-sdk-python/issues/10#issuecomment-5773539291). Submitted for maintainer consideration; not yet merged. Validation used offline fixtures and a local HTTP server, not live Jev benchmarks.

### Selected public projects

#### [BLE Helper](https://github.com/vonpanda/BLE_Helper)

An Android BLE debugging companion for hardware development. Discover devices, inspect GATT services, read and write characteristics, subscribe to notifications, and export activity logs.

`Flutter` `Dart` `BLE` `BLoC` `Drift`

[Overview](https://github.com/vonpanda/BLE_Helper#readme) · [BLE implementation](https://github.com/vonpanda/BLE_Helper/tree/main/lib/services/ble) · [Tests](https://github.com/vonpanda/BLE_Helper/tree/main/test)

**Status:** Android is the current target. DFU is an adapter scaffold; an actual update backend still needs integration and device validation.

#### [schematic-mcp](https://github.com/vonpanda/schematic-mcp)

Structured hardware schematic context for developer tools via MCP. Query KiCad components, pins, and nets, with an example that compares firmware pin expectations against schematic connectivity.

`Python` `KiCad` `MCP` `Connectivity graph`

[Overview](https://github.com/vonpanda/schematic-mcp#readme) · [Pin validation demo](https://github.com/vonpanda/schematic-mcp/blob/main/docs/firmware-validation-demo.md) · [Tests](https://github.com/vonpanda/schematic-mcp/tree/main/tests)

**Status:** Alpha, with a modern KiCad adapter. Other EDA formats and complete cross-sheet connectivity remain planned work.

### Earlier C++ and Qt work

| Project | Code to explore |
| --- | --- |
| [C++ TCP Chatroom](https://github.com/vonpanda/chatroom-C-) | Linux sockets, epoll event loops, client connections, and message broadcasting |
| [Qt Network Sign-in](https://github.com/vonpanda/QT_webSignin) | Qt Widgets, signals and slots, QTcpSocket, system tray integration, and configuration I/O |

These repositories preserve early learning implementations for code reading and discussion.

## 简体中文

我做连接软件与硬件的开发工作：从设备数据采集、通信协议，到桌面端监控与调试工具。曾从事 GPU 虚拟化研发，并有嵌入式系统集成经验。

### 开发方向

- **桌面软件** — Qt / PyQt 界面、设备状态监控、Windows 设备输入处理与跨平台打包。
- **设备通信** — 串口、BLE GATT / HID、MODBUS RTU、传感器数据采集与软硬件联调。
- **工程工具** — Python 自动化、MCP 集成、原理图连接与固件引脚映射检查。

### 当前关注

连接设备与固件工作流和 AI Agent 工具：通过 MCP 提供结构化硬件上下文，开发 Python SDK 集成，并明确处理不确定结果。目前正在探索类型化决策模型在路由和运维分流中的应用，尚未在设备数据上完成 Jev 基准评测。

### 开源贡献

- **TypeSafe Python SDK — HTTP/2 文档：** 准备了同步、异步客户端示例，并检查并发请求的连接生命周期。[补丁](https://github.com/typesafe-ai/typesafe-sdk-python/compare/main...vonpanda:typesafe-sdk-python:docs/http2-client-examples) · [上游讨论](https://github.com/typesafe-ai/typesafe-sdk-python/issues/10#issuecomment-5773539291)。已提交供维护者考虑，尚未合并。验证使用离线样本和本机 HTTP 服务，不代表真实 Jev 性能测试。

### 精选公开项目

#### [BLE Helper](https://github.com/vonpanda/BLE_Helper)

面向硬件开发的 Android BLE 调试助手。支持设备扫描、GATT 服务浏览、特征值读写、通知订阅和日志导出。

`Flutter` `Dart` `BLE` `BLoC` `Drift`

[项目介绍](https://github.com/vonpanda/BLE_Helper/blob/main/README.zh-CN.md) · [BLE 通信层](https://github.com/vonpanda/BLE_Helper/tree/main/lib/services/ble) · [测试代码](https://github.com/vonpanda/BLE_Helper/tree/main/test)

**当前状态：** 以 Android 为目标平台；DFU 为适配器框架，尚需接入实际升级后端并完成真机验证。

#### [schematic-mcp](https://github.com/vonpanda/schematic-mcp)

通过 MCP 为开发工具提供结构化的原理图信息。可查询 KiCad 器件、引脚和网络，包含固件预期引脚与原理图连接关系的对照示例。

`Python` `KiCad` `MCP` `Connectivity graph`

[项目介绍](https://github.com/vonpanda/schematic-mcp#readme) · [引脚校验示例](https://github.com/vonpanda/schematic-mcp/blob/main/docs/firmware-validation-demo.md) · [测试代码](https://github.com/vonpanda/schematic-mcp/tree/main/tests)

**当前状态：** alpha，已实现现代 KiCad 文件适配；其他 EDA 格式与完整跨页连接仍在规划中。

### 早期 C++ 与 Qt 实践

| 项目 | 代码阅读重点 |
| --- | --- |
| [C++ TCP 聊天室](https://github.com/vonpanda/chatroom-C-) | Linux Socket、epoll 事件循环、客户端连接与消息广播 |
| [Qt 校园网登录工具](https://github.com/vonpanda/QT_webSignin) | Qt Widgets、信号槽、QTcpSocket、系统托盘与配置读写 |

这些仓库保留了早期学习实现，供阅读代码与交流思路。

[Back to top · 返回顶部](#冯汉昱--hanyu-feng)
