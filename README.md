# improved-octo-parakeet
code
# STM32F103C8T6 基于 ucosiii 操作系统的收音机黑电台检测系统
该项目是一个使用 STM32F103C8T6 控制器，在 ucosiii 操作系统使用HAL库下实现的收音机黑电台检测模块，使用 Keil5 开发工具，同时包含 ESP8266 WiFi 模块、TEA5767 收音机模块和 SD 卡模块。
## 硬件需求
- STM32F103C8T6 控制器
- ESP8266 WiFi 模块
- TEA5767 收音机模块
- SD 卡模块
## 软件依赖
- Keil5 开发工具
- ucosiii 操作系统
## 硬件连接
以下是硬件连接图：
±-----------+  

| STM32F1  |  

| 103C8T6  | ±------------------------+  

| MCU      | | ESP8266 WiFi |  
|          | |              |  
| PA.9     |—|RX            |  
| PA.10    |—|TX            |  
|          | ±------------------------+  
|          | |TEA5767     |  
| PB.6     |—|SCL         |
| PB.7     |—|SDA         |
|          | ±------------------------++
|          | | SD 卡模块 |  |
| PA.4     |—|CS |         |
| PA.5     |—|CLK |        |
| PA.6     |—|MISO |       |
| PA.7     |—|MOSI |       |
±-----------+ ±------------------------+
| PB11     |-|CS |         |
| PB10     |-|DC |         |
| PB12     |-|RES|         |
| PB15     |-|SDA|         |
| PB13     |-|SCK|         |
±-----------+ ±------------------------+
