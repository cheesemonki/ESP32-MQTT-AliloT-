# ESP32-MQTT-AliloT-

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
SERVER = 'xxxxxxxxxxxxxxxx'  # mqtt服务器地址
CLIENT_ID = "xxxxxxxxxxxx"  # clientId
username = 'xxxxxxxxxx'  # 用户名
password = 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxx'  # 密码
