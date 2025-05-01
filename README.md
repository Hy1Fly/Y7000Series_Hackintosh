# Y7000Series_Hackintosh <img src="https://img.shields.io/badge/macOS-Ventura/Sonoma-blue?style=flat&logo=apple" alt="macOS"> <img src="https://img.shields.io/badge/OpenCore-0.9.8+-green?style=flat" alt="OpenCore">

为联想拯救者Y7000系列笔记本提供Hackintosh EFI配置

![Hackintosh Preview](https://example.com/preview.jpg) <!-- 可替换为实际效果图链接 -->

## 📖 目录
- [概述](#-概述)
- [兼容性](#-兼容性)
- [BIOS设置指南](#-bios设置指南)
- [功能支持](#-功能支持)
- [快速优化](#-快速优化)
- [致谢](#-致谢)

## 🌟 概述
本仓库为联想拯救者Y7000系列笔记本（2018-2020款）提供经过验证的Hackintosh EFI配置，支持macOS 10.13至最新版本的系统OTA升级。项目基于OpenCore引导，持续维护i5-9代处理器系列。

---

## 🖥️ 兼容性

### 支持系统版本
macOS 10.13 High Sierra ~ macOS 15.0 Sequoia（需自行测试新版本兼容性）

### 适配机型
- **2018款**  
  Y7000 / Y7000P / Y9000K
- **2019款**  
  Y7000 / Y7000P / Y9000K
- **2020款**  
  Y7000 / Y7000P / Y9000K

---

## ⚙️ BIOS设置指南
**必须完成以下BIOS配置：**
1. 进入BIOS设置（开机按F2）
2. 启用 `UEFI Boot`
3. 禁用 `Secure Boot`
4. 设置SATA模式为 `AHCI`
5. 执行 **[BIOS高级设置一键修改脚本](https://github.com/xiaoMGitHub/LEGION_Y7000Series_Insyde_Advanced_Settings_Tools)**  
   （脚本将解锁隐藏设置项）

---

## ✅ 功能支持
### 完美工作
- ⌨️ 内置键盘（含数字键盘）| 💤 睡眠唤醒（支持键盘/鼠标/电源键唤醒）
- 🔊 AppleHDA音频（扬声器 & 耳机自动切换）| 🔋 电池状态监测
- 🌞 屏幕背光控制 | 🖥️ 核显加速（Intel UHD Graphics）
- 🌐 有线网络 | 🖱️ 触控板全手势支持
- 🚀 CPU变频 | 🖨️ 随航（有线/无线）
- 📷 内置摄像头 | 🛏️ 深度休眠唤醒（hibernatemode 25）

### 有限支持
- 🖥️ HDMI输出（需特定机型）  
  *建议使用DisplayLink方案外接显示器*
- 🔌 Type-C扩展坞（功能受限）  
- ✈️ 隔空投送（需更换白苹果网卡）  
  *推荐使用BCM94360CD网卡*
- ⚡ NVIDIA独显（仅部分型号）  
  *通过OCLP可驱动GTX1060以下显卡（不推荐）*

---

## 🚀 快速优化
执行以下命令进行系统优化（包含缓存重建、权限修复等）：
```bash
sudo sh -c "$(curl -fsSL https://gitee.com/xiaoMGit/Y7000Series_Hackintosh_Fix/raw/master/Script/Optimize.sh)"
```

---

## 🙏 致谢
特别感谢 [@xiaoMGithub](https://github.com/xiaoMGitHub) 的持续贡献与技术支持！  
(*ゝω・)ﾉ 您的支持是项目前进的动力！

---

**📢 重要提示**  
- 安装前请务必备份原始EFI
- 推荐使用[Hackintool](https://github.com/headkaze/Hackintool)进行个性化调整
- 遇到问题请先查阅[讨论区](https://github.com/your_repo/issues)
