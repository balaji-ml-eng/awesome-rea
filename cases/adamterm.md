# AdamTerm：研究 Ghostty 外壳后做自己的终端

[← 返回案例目录](../README.md) · 应用实践

- **作者 / 来源归属：** AdamLinCodes
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Ghostty 1.3.1 macOS app bundle

## 想解决什么问题

终端核心、原生窗口、菜单和服务之间怎么分工？

## REA 具体做了什么

使用 REA 检查 Mach-O、plist、签名、Objective-C 元数据、Interface Builder 与动态库解析；该路径未使用 Hopper/Ghidra。

## 公开成果

以下是来源作者报告的成果：

作者以 AppKit + SwiftTerm 做了带原生标签页的精简 macOS 终端，并提供自检命令。

## 局限与未验证项

使用 SwiftTerm 而非重建 Ghostty 的 Zig 核心；分屏、搜索栏、配置文件、快捷终端等未实现。

## 可以借鉴什么

包元数据和界面资源就能回答一部分架构问题，不必一开始深度反编译。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> A minimal macOS terminal built by reverse-engineering Ghostty 1.3.1 with REA

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/AdamLinCodes/AdamTerm/blob/5278f12a7e885c793bbf5aeb567950fa17798ba5/README.md)
- [项目 / 演示](https://github.com/AdamLinCodes/AdamTerm)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
