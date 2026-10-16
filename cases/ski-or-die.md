# Ski or Die：用 Rust 重建 Snowball War

[← 返回案例目录](../README.md) · 游戏实践

- **作者 / 来源归属：** tuunanet
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** DOS 版 Ski or Die 的 Snowball War 小游戏

## 想解决什么问题

怎样从旧 DOS 程序恢复投掷、碰撞、刷怪与计分规则？

## REA 具体做了什么

REA CLI + Ghidra 16 位适配器检查解包后的 MZ 装载镜像，再通过调用者声明的代码种子和 trace/function/search 调查各模块。

## 公开成果

以下是来源作者报告的成果：

作者公开了 Rust + SDL2 可玩重建、行为规格、逆向笔记与资产提取工具。

## 局限与未验证项

只重建 Snowball War；无声音播放、无 DOS 原版并排运行对照；帧率与 PRNG 有近似。需读者自己的游戏副本生成素材。

## 可以借鉴什么

先将行为写成有地址证据的规格，再重写；逐项标记近似行为。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> Every analysis call therefore ran through the REA CLI

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/tuunanet/rea-ski-or-die-reconstruction/blob/0eac0671c90e21a16e663da7772b60710101ef7f/README.md)
- [项目 / 演示](https://github.com/tuunanet/rea-ski-or-die-reconstruction)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
