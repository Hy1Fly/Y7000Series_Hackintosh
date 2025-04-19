# Y7000Series_Hackintosh
给联想拯救者Y7000系列提供HackintoshEFI
## 概述

本EFI适用于LENOVO 拯救者Y7000系列笔记本
并且会提及一些注意事项

感谢@xiaoMGithub
(*ゝω・)ﾉThanks!

## 适用系统
 
MacOS 10.13~15.0

## 适用型号

- Y7000/Y7000P/Y9000K-2018
- Y7000/Y7000P/Y9000K-2019
- Y7000/Y7000P/Y9000K-2020

## BIOS设置
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
- Nvdia显卡（据说可以使用OCLP进行驱动，但只支持GTX1060以下，并且不推荐！！！）
- 隔空投送（使用白果卡应该就可以工作了）

## 优化命令
```
sudo sh -c "$(curl -fsSL https://gitee.com/xiaoMGit/Y7000Series_Hackintosh_Fix/raw/master/Script/Optimize.sh)"
```