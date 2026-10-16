# Ledger Reborn：研究 QuickBooks 后做本地账本

[← 返回案例目录](../README.md) · 应用实践

- **作者 / 来源归属：** lxistired
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** QuickBooks Desktop for Mac

## 想解决什么问题

如何理解桌面会计工作流，并做独立本地应用？

## REA 具体做了什么

作者声明用 REA 调查 QuickBooks，再实现本地 SQLite 会计引擎与桌面界面，并公开 CASE_STUDY。

## 公开成果

以下是来源作者报告的成果：

公开 preview 包、源码和案例记录；作者列出发票、付款、库存、银行对账和报表等已实现流程。

## 局限与未验证项

仍为 preview、单用户单机 USD；工资、报税、在线银行、多币种和完整 QuickBooks 文件迁移未实现；未完成全面交互/像素等价验证。

## 可以借鉴什么

把逆向调查落到可检查的业务流程，同时写清财务规则和不支持的业务。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> We used REA to investigate QuickBooks Desktop for Mac and independently implement a desktop accounting tool.

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/lxistired/ledger-reborn/blob/d7f6b8a1f4ad6c4ae8b10100d1c93cf15940c21d/README.md)
- [项目 / 演示](https://github.com/lxistired/ledger-reborn)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
