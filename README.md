# Y7000Series_Hackintosh
给联想拯救者Y7000系列提供HackintoshEFI
## 概述

本文的目的是让 LENOVO 拯救者系列笔记本电脑尽量完美的使用上 MacOS。


## 适用系统

macOS Ventura 13.x  
MacOS Monterey 12.x  
MacOS Big Sur 11.x  
MacOS Catalina 10.15.x  
MacOS Mojave 10.14.x  
MacOS High Sierra 10.13.6 (17G2112)

## 适用型号

- Y7000/Y7000P/Y9000K-2018
- Y7000/Y7000P/Y9000K-2019
- Y7000/Y7000P/Y9000K-2020
- Y530/Y540/Y545/Y730/Y740
- Legion 5i/Legion 7

## BIOS确保设置
- 启用UEFI启动。
- 禁用安全启动。
- SATA模式设置为AHCI。
- 执行[一键修改BIOS脚本。](https://github.com/xiaoMGitHub/LEGION_Y7000Series_Insyde_Advanced_Settings_Tools)

## 正常工作的功能
- 支持任意版本系统OTA升级到最新系统
- 内置键盘以及数字键盘
- 原生USB3.0/USB2.0 
- AppleHDA原生音频，包括耳机
- 内置摄像头
- 原生电源管理
- 电池状态
- 背光控制
- 背光键盘
- 核显驱动
- 有线以太网卡
- Mac App Store正常运行
- CPU变频
- 睡眠唤醒（鼠标，键盘、电源键唤醒均正常，并且继续维护i5-9代系列）
- 无线网络与蓝牙（OCLP补丁可以驱动原生网卡，但依旧建议更换白果卡BCM94360CD）
- 触控板 （全系支持全手势）
- 随航（有线/无线）
- 支持休眠唤醒（hibernatemode 25）

## 不能完美使用或者需要其它工具的功能
- HDMI
- Type-C(扩展坞)
- 外接显示器(Displaylink)

## 优化命令
```
sudo sh -c "$(curl -fsSL https://gitee.com/xiaoMGit/Y7000Series_Hackintosh_Fix/raw/master/Script/Optimize.sh)"
```