# Human beta1.0 MCP Bridge

这是连接 Human 身体和 AI 的桥梁。

## 作用

Bridge 负责把 ESP32 的信息转换成 MCP 工具，让 AI 可以访问。

当前工具：

- get_esp32_status
  - 获取设备状态

- get_touch_state
  - 获取当前触摸状态

- test_touch_realtime
  - 测试触摸变化

## 当前流程

ESP32
↓
WiFi
↓
HTTP 状态接口
↓
Human Bridge
↓
MCP
↓
AI

## 目前阶段

beta1.0 先完成触摸感知。

不要急着堆功能，先让第一条感官稳定工作。