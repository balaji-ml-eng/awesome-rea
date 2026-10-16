# rea-groundtruth：对照已知源码找分析盲点

[← 返回案例目录](../README.md) · 分析与评测

- **作者 / 来源归属：** UnknownHacker1
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** MongoDB Compass 1.43.4 及手写 Electron fixtures

## 想解决什么问题

工具报告零个 IPC/窗口时，是程序真的没有，还是分析漏掉了？

## REA 具体做了什么

使用 REA 6.4.0 分析源码已知的应用，再用不同 webpack 包装形式的最小样本做对照。

## 公开成果

以下是来源作者报告的成果：

作者公开一键复现：特定 webpack 形态的 Electron API 没被识别，并记录签名后 ASAR integrity mismatch 的处理方式。

## 局限与未验证项

报告针对 Windows 11 与 REA 6.4.0 的特定构建；后续版本可能修复。这里没有把历史发现表述为最新版本仍存在的 bug。

## 可以借鉴什么

零发现不等于不存在；有源码的 fixtures 能验证分析器覆盖范围。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> Tested with rea-agents 6.4.0 on Windows 11 x64, Node 22.22.

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/UnknownHacker1/rea-groundtruth/blob/5b48f366368c9fbe2abaaab810aba6814c27190b/README.md)
- [项目 / 演示](https://github.com/UnknownHacker1/rea-groundtruth)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
