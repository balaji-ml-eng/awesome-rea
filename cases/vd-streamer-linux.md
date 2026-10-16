# Virtual Desktop Streamer：替换平台层实现 Linux 移植

[← 返回案例目录](../README.md) · 硬件与兼容

- **作者 / 来源归属：** cudanexus
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Virtual Desktop 官方 macOS 和 Windows 安装包

## 想解决什么问题

如何保留协议库，把采集、编码、音频和输入换成 Linux 实现？

## REA 具体做了什么

作者声明使用 Claude Code + REA 分析两种安装包，复用读者自行提供的 macOS 协议库，重写 Linux 平台层。

## 公开成果

以下是来源作者报告的成果：

公开 Linux 移植源码、构建与模拟头显测试，使用 PipeWire/X11、GStreamer 和 uinput。

## 局限与未验证项

没有真实头显、Wi-Fi 和 GPU 编码器测试；不支持 Windows streamer 的 SteamVR/OpenXR 游戏功能。依赖厂商协议库，不能理解为完整独立协议重写。

## 可以借鉴什么

兼容移植可以聚焦平台边界；模拟设备测试和真实硬件验收需分别报告。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> This port was built by Claude Code (Claude Opus) with the REA reverse-engineering tools

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/cudanexus/vd-streamer-linux/blob/e65c302f13639f044742bdc4951ab1a424c1c929/README.md)
- [项目 / 演示](https://github.com/cudanexus/vd-streamer-linux)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
