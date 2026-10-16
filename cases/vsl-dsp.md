# VSL-DSP：把厂商库分析用于声卡 DSP 工具

[← 返回案例目录](../README.md) · 硬件与兼容

- **作者 / 来源归属：** grisuno
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** PreSonus Universal Control 的 libucnet.so 与 libfatchannelplugins.so

## 想解决什么问题

厂商控制程序如何发现设备、注册参数和表示增益？

## REA 具体做了什么

通过 LazyOwn 的 rea 扩展驱动 REA + Ghidra 分析厂商库，保留 Evidence envelope 并形成协议与参数规格。

## 公开成果

以下是来源作者报告的成果：

作者将调查结果用于 dB 命令、参数命名和线性/dB 转换，并提供 CMocka 测试。

## 局限与未验证项

REA 的作用限定为部分厂商库发现与后续改进，不应把整个驱动归功于 REA；mute wire code 没有恢复。

## 可以借鉴什么

协议调查适合补齐现有项目中的具体缺口，未知控制码要保持未知。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> lazyaddon, which drives REA (Reverse Engineer Anything) with Ghidra 12.1.4

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/grisuno/VSL-DSP/blob/e619f0877ffca3c183be37cdd9474f2d7e348ad5/README.md)
- [项目 / 演示](https://github.com/grisuno/VSL-DSP)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
