# Notion：追踪 Electron 富文本剪贴板桥

[← 返回案例目录](../README.md) · 官方案例

- **作者 / 来源归属：** REA 官方案例团队；原项目作者见来源
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** Notion Desktop 7.6.1 的 app.asar，以及另一个时间点缓存的网页编辑器模块

## 想解决什么问题

网页编辑器如何通过桌面端写入富文本剪贴板？

## REA 具体做了什么

REA 静态分析 tab preload，定位 context bridge 与 IPC invoke；随后直接阅读打包代码，补齐 clipboard API、channel 和主进程接收路径。

## 公开成果

以下是来源作者报告的成果：

公开案例展示了 renderer → preload → IPC → main 的源码级解释，以及独立模块探针中的富文本标记与 Markdown 表格处理。

## 局限与未验证项

REA 图没有自动解析出完整 clipboard channel 链；网页编辑器与桌面包不是同版本运行时样本，没有捕获同版本真实复制粘贴。

## 可以借鉴什么

将 REA 实际返回的结构、人工读代码补充的结论、独立探针结果分开。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> The published npm REA 4.1.0 package inspected the saved tab preload on 7 October 2026

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/morluto/rea/blob/42fc6c53ae188978deb3bedfe88287b6b316ba22/website/evidence/notion-clipboard.md)
- [项目 / 演示](https://rea.tools/showcase/notion/)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
