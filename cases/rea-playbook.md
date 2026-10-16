# rea-playbook：把 Electron Evidence 变成可读报告与重建

[← 返回案例目录](../README.md) · 学习与复现

- **作者 / 来源归属：** jinshi666888
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** 仓库自带的八文件最小 Electron 示例

## 想解决什么问题

拿到巨大 Evidence JSON 后，怎样提取可读事实并验证重建？

## REA 具体做了什么

固定 REA 6.3.0，提供 analyze → extract → verify 命令链，另有 MCP handshake 与真实工具调用 probe。

## 公开成果

以下是来源作者报告的成果：

公开脱敏 Evidence fixture、file:line 报告、recreate 与断言；作者报告 10/10 重建检查通过。

## 局限与未验证项

离线 demo 只读取已有 fixture，不能冒充新运行 REA；自建小目标也不能代表复杂商业应用。

## 可以借鉴什么

入门可以从可控小样本开始，把证据、可读规格和回归检查串起来。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> npm run analyze will fetch rea-agents@6.3.0 on first use via npx fallback.

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/jinshi666888/rea-playbook/blob/0ad65a85139025f32402be13ed64c8003e39b00a/README.md)
- [项目 / 演示](https://github.com/jinshi666888/rea-playbook)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
