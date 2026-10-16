# Desktop Games：把砸桌面小游戏移植到 macOS 和浏览器

[← 返回案例目录](../README.md) · 游戏实践

- **作者 / 来源归属：** ucodia
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Gemtree 2000 年 Desktop Games / Stress Reducers 的 Windows 程序

## 想解决什么问题

怎样理解 Peter 解释器和程序树，并移植交互与资源？

## REA 具体做了什么

作者使用 Claude Code、REA 与 Ghidra；REA 用于解释器中图像压缩、资源布局、计时、精灵运动、声音与坐标规则的调查；配套 Python 工具处理程序树和资源。

## 公开成果

以下是来源作者报告的成果：

公开仓库包含 Swift macOS 版、浏览器版、反编译程序树及资源处理脚本。

## 局限与未验证项

作者注明使用真彩色而非原调色板，并调整了阴影实现；案例收录不表示本仓库验证了完整兼容性或第三方素材的再分发权。

## 可以借鉴什么

遇到嵌入解释器的程序，要区分解释器、程序树和资源三个层次。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> The interpreter was decompiled with REA

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/ucodia/desktop-games-nostalgia/blob/27946dfe49d4a9b522dfe017c14eefbc0ca40b2a/README.md)
- [项目 / 演示](https://github.com/ucodia/desktop-games-nostalgia)
- [补充来源 1](https://ucodia.github.io/desktop-games-nostalgia/)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
