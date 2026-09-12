<picture>
  <img alt="Hanyu Feng — Desktop software and device connectivity" src="https://raw.githubusercontent.com/vonpanda/vonpanda/main/assets/header.svg" width="100%">
</picture>

# 冯汉昱 · Hanyu Feng

**C++ / Qt / Python · 桌面工具与设备通信**

我做连接软件与硬件的开发工作：从设备数据采集、通信协议，到桌面端监控与调试工具。曾从事 GPU 虚拟化研发，目前关注上位机软件、嵌入式联调，以及帮助工程师理解硬件的工具。

I build desktop tools and software that communicate with devices, with experience in GPU virtualization and embedded integration.

### 开发方向

- **桌面软件** — Qt / PyQt、设备状态显示、Windows 设备输入处理与跨平台打包。
- **设备通信** — 串口、BLE GATT / HID、MODBUS RTU，以及传感器数据采集与联调。
- **工程工具** — Python 自动化、MCP 集成、原理图与固件引脚映射检查。

### 公开项目

#### [BLE Helper](https://github.com/vonpanda/BLE_Helper)

面向硬件调试的 Android BLE 助手。围绕设备扫描、连接、GATT 浏览、特征值读写、通知与日志导出组织交互。

`Flutter` `Dart` `BLE` `BLoC` `Drift`

[阅读项目介绍](https://github.com/vonpanda/BLE_Helper#readme) · [查看 BLE 通信层](https://github.com/vonpanda/BLE_Helper/tree/main/lib/services/ble) · [查看测试](https://github.com/vonpanda/BLE_Helper/tree/main/test)

当前以 Android 为目标平台；DFU 为适配器框架，尚需接入并验证实际升级后端。

#### [schematic-mcp](https://github.com/vonpanda/schematic-mcp)

将 KiCad 原理图中的器件、引脚和网络转换为可查询的结构化数据，通过 MCP 提供给开发工具；包含固件预期引脚与原理图连接关系的对照示例。

`Python` `KiCad` `MCP` `Connectivity graph`

[阅读项目介绍](https://github.com/vonpanda/schematic-mcp#readme) · [查看引脚校验示例](https://github.com/vonpanda/schematic-mcp/blob/main/docs/firmware-validation-demo.md) · [查看测试](https://github.com/vonpanda/schematic-mcp/tree/main/tests)

当前为 alpha，已实现现代 KiCad 文件适配；其他 EDA 格式与完整跨页连接仍在规划中。

### 早期 C++ 与 Qt 实践

| 项目 | 代码阅读重点 |
| --- | --- |
| [C++ TCP 聊天室](https://github.com/vonpanda/chatroom-C-) | Linux Socket、epoll 事件循环、客户端连接与消息广播 |
| [Qt 校园网登录工具](https://github.com/vonpanda/QT_webSignin) | Qt Widgets、信号槽、QTcpSocket、系统托盘与配置读写 |

这些仓库保留了早期学习实现，供阅读代码与交流思路。
