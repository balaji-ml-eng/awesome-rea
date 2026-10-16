# Aegis：从 Android APK 找出动态验证码算法

[← 返回案例目录](../README.md) · 官方案例

- **作者 / 来源归属：** REA 官方案例团队；原项目作者见来源
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Aegis Authenticator 3.4.3 Android APK

## 想解决什么问题

每 30 秒变化的六位登录码是怎么计算的？

## REA 具体做了什么

REA Android 分析定位生成、显示和复制相关方法，阅读 HOTP/TOTP 计算，再编写可调整时钟的浏览器演示。

## 公开成果

以下是来源作者报告的成果：

官方页面报告：提取方法与独立实现对照 133 个用例，并核对 RFC 6238 的六个 SHA-1 参考样例。

## 局限与未验证项

范围是验证码生成计算；不代表完成密钥库、加密存储或整款应用的重建。本仓库没有复跑这些用例。

## 可以借鉴什么

选一个可独立验证的小功能，用公开标准测试向量约束实现。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> Inspected with REA 6.1.0 on 9 October 2026.

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/morluto/rea/blob/42fc6c53ae188978deb3bedfe88287b6b316ba22/website/public/showcase/aegis/index.html)
- [项目 / 演示](https://rea.tools/showcase/aegis/)
- [补充来源 1](https://github.com/beemdevelopment/Aegis)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
