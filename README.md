# 🛰️ 代号“夜鹭”小时钟

![配置](https://img.shields.io/badge/Platform-ESP32--C3-orange?logo=espressif)
![开源协议](https://img.shields.io/badge/License-MIT-blue)
![框架](https://img.shields.io/badge/Framework-Arduino-pro?logo=Arduino)

## ✨ 特点
- 🕒 **NTP时间同步**: 开机时自动从苹果服务器获取时间
- 🌤️ **天气功能**: 开机时从心知天气获取数据
- 🌊 **灵动UI**: 界面之间切换如德芙般丝滑
- 🌙 **自动省电**: 可设置秒钟后息屏，自动断网机制
- 📆 **农历功能**: 开机自动获取当天的农历数据
- 📟 **哔哩哔哩播放量** 开机自动获取指定视频的播放量

## 🛠️ 硬件总览
- **处理器**: ESP32-C3
- **屏幕**: SSD1306 128x32 OLED
- **按钮**: 5个 (Confirm, Left, Right, Back, Sleep)

## 🚀 开始个性化
1. 在你的电脑上安装git并输入:
   ```cmd
   git clone https://github.com/Jihao2048/Heron-Clock.git
2. 在PlatformIO里面打开这个文件夹
3. 编辑`include/conf.h`来更改你的信息 :
   ```cpp
   //在这里填写你家的WiFi和密码
   #define WIFI_SSID ""
   #define WIFI_PASS ""
   //找你喜欢的哔哩哔哩视频复制bvid到这里
   String bvid = "";
   //建议大家去申请自己的token https://alapi.cn/api/32/api_document
   String lunartoken = "";
   //建议大家去申请自己的key https://www.seniverse.com/
   String weatherkey = "";
   //填写你家在哪个市，例如shenzhen，或者weifang
   String location = "";
   //根据你屏幕的实际垂直偏移像素调整
   int pixeloffset = 2;

## 📷 图片

### 🕒 主界面
时间，日期，还有天气，温度。
<p align="center">
  <img src="1.jpg" width="400">
</p>

### 📆 中国农历
丙午马年三月十四周几运势
<p align="center">
  <img src="2.jpg" width="400">
</p>

---
> 我的[哔哩哔哩账号](https://space.bilibili.com/2121656213) 附带演示和使用说明。

> 在干燥适宜温度环境下使用，仅进行正常操作（静置、携带、充电、烧录官方程序）。对于非正常使用造成的任何损害，本人(即项目作者)不承担责任。
