# REA on REA：分析工具自身并检验预测

[← 返回案例目录](../README.md) · 分析与评测

- **作者 / 来源归属：** az9713
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** 已安装的 rea-agents 6.3.0 包

## 想解决什么问题

REA 如何选择原生分析 provider，又怎样判断 provider 不可用？

## REA 具体做了什么

REA 静态分析自身五个目录，代理先写可证伪预测，再运行 doctor，最后查看源码答案并自评。

## 公开成果

以下是来源作者报告的成果：

公开完整过程与测试回执；作者报告四个回答都只部分正确，八个 Ghidra 检查结果中预测错了三个。

## 局限与未验证项

单次自评，且 doctor 测试不等同于 open_binary 测试；存在安装包与源码 checkpoint 差异。

## 可以借鉴什么

把听起来合理的解释转化为能验证的预测，并公开失败。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> REA analyzed 5 folders of the installed rea-agents 6.3.0 package with analyze_javascript_application.

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/az9713/REA-demo/blob/d01fc8ac812abaddae85e86f7ff116cd8b9b52c3/README.md)
- [项目 / 演示](https://github.com/az9713/REA-demo)
- [补充来源 1](https://az9713.github.io/REA-demo/rea-on-rea-receipt.html)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
