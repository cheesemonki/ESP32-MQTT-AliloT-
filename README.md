
# ESP32 MQTT 项目

## 项目简介

本项目基于ESP32开发板，通过MQTT协议与阿里云物联网平台进行通信。项目实现了通过MQTT协议接收和发送消息，控制ESP32上的LED灯。

## 硬件需求

- ESP32开发板
- DHT11温湿度传感器
- LED灯

## 软件需求

- Micropython固件
- umqtt.simple库

## 项目配置

### WiFi配置

修改以下代码中的 `SSID` 和 `PASSWORD` 为您自己的WiFi名称和密码。

```python
SSID = "MONKI"  # 填写自己的WIFI名称
PASSWORD = "88888888"  # 填写自己的WIFI密码
```

### MQTT配置

修改以下代码中的 `SERVER`, `CLIENT_ID`, `username`, 和 `password` 为您自己的MQTT服务器地址、客户端ID、用户名和密码。

```python
SERVER = 'a1pwuxxxxxxiot-as-xxxxxxxhai.aliyuncs.com'  # mqtt服务器地址
CLIENT_ID = "a1xxxxxxxxxOu.esp32|securemode=2,signxxxx=hmacsha256,timestaxxxxxxxx72757040|"  # clientId
username = 'esp32&a1pxxxxxxxxvOu'  # 用户名
password = '397xxxxxx4055c2fd7dxxxxxa83fdaxxxxxx34daxxxxxx0fd83dxxxxxx0'  # 密码
```

### 运行项目

将 `main.py` 文件上传到ESP32开发板并运行。程序将自动连接WiFi，并连接到MQTT服务器。LED灯的状态可以通过MQTT消息进行控制。

### 其他说明

如需更多信息，请参阅项目代码中的注释。
