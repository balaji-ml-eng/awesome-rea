# hexgrab：从 PowerToys 二进制研究取色器

[← 返回案例目录](../README.md) · 应用实践

- **作者 / 来源归属：** iammukeshm
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Microsoft PowerToys 随发行版提供的取色器二进制

## 想解决什么问题

全局快捷键、像素取色和剪贴板怎样配合？

## REA 具体做了什么

作者用 REA 分析已发布二进制，再利用公开源码逐条核对发现，使用 .NET 10 / WPF 独立实现精简取色器。

## 公开成果

以下是来源作者报告的成果：

公开源码与 docs/rea-findings.md；作者报告 9 条发现中 8 条完全正确。

## 局限与未验证项

仅在单显示器、125% 缩放下测试；混合 DPI 多显示器未做真实硬件验证。8/9 是作者对该次调查的核对，不是 REA 通用准确率。

## 可以借鉴什么

选择源码公开的软件做逆向练习，有条件检查工具到底对了多少。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> to study how the Color Picker in Microsoft PowerToys works from its shipped binaries

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/iammukeshm/hexgrab/blob/511c58078776af4fb0d2e3601e098f98e9f90c9a/README.md)
- [项目 / 演示](https://github.com/iammukeshm/hexgrab)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
