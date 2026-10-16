# rea-lab：测量 REA 对 Windows 逆向任务的实际帮助

[← 返回案例目录](../README.md) · 分析与评测

- **作者 / 来源归属：** pablodiazjorge
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Windows 小型挑战、更大含诱饵二进制及真实开源程序

## 想解决什么问题

加上 REA 后，代理解决任务的成功率、耗时和成本怎样变化？

## REA 具体做了什么

搭建 Windows + Ghidra 环境，做预注册对照研究，核验引用 Evidence，公开 writeups、环境与上游修复。

## 公开成果

以下是来源作者报告的成果：

Study 1 报告两组均解出 28/30；Study 2 为无 REA 11/24、用 REA 4/24；Study 3 为 71/72 与 68/72。作者报告 REA 组耗时与成本更高。

## 局限与未验证项

后两组差异未达来源所用统计检验的显著水平；样本、任务、模型、版本都受限，不能推广成 REA 对所有任务无效。数值按公开 README 转述，未复跑。

## 可以借鉴什么

评估工具时同时看对照组、任务分布、成本与证据质量。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> Study 1, preregistered: on ten small Windows crackmes, rea did not change how many Claude Code solved

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/pablodiazjorge/rea-lab/blob/8796545134a00023b0fba3d75dbbaf77a9be68d8/README.md)
- [项目 / 演示](https://github.com/pablodiazjorge/rea-lab)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
