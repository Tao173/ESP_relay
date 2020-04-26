# 开关模块

本开关模块为自己家装修使用，只支持零火。没有单火需求所以也没有单火版。

![image](https://github.com/qlwz/esp_relay/blob/master/file/images/正面.png)
![image](https://github.com/qlwz/esp_relay/blob/master/file/images/反面.png)
![image](https://github.com/qlwz/esp_relay/blob/master/file/images/成品.png)
![image](https://github.com/qlwz/esp_relay/blob/master/file/images/LED状态.png)

开关模块以ESP-01M为基础实现了一路、二路、三路并附带面板LED指示灯及射频功能

- 一路：[一路开关模块详细资料](https://github.com/qlwz/esp_relay/tree/master/file/1%E8%B7%AF%E5%BC%80%E5%85%B3%E6%A8%A1%E5%9D%97)
- 二路：[二路开关模块详细资料](https://github.com/qlwz/esp_relay/tree/master/file/2%E8%B7%AF%E5%BC%80%E5%85%B3%E6%A8%A1%E5%9D%97)
- 三路：[三路开关模块详细资料](https://github.com/qlwz/esp_relay/tree/master/file/3%E8%B7%AF%E5%BC%80%E5%85%B3%E6%A8%A1%E5%9D%97)

## IO对应：  
按键：  
L1：GPIO4  
L2：GPIO9  
L3：GPIO10  
面板指示灯：  
S1：GPIO0  
S2：GPIO2  
S3：GPIO15  

## 射频
为什么需要射频？  
不想因为WIFI或者HA等设备出故障的时候影响日常生活。  
射频为软件解码支持433MHz和315MHz  

# 固件

## 特性

本固件使用开关模块硬件为基础，实现以下功能:

- [x] 单独控制开关
- [x] 支持普通开关、自复位开关
- [x] 支持三档筒灯
- [x] 支持射频
- [x] OTA在线升级
- [x] WEB配置页面
- [x] MQTT服务器连接控制
- [x] 通过MQTT连入Home Assistant
