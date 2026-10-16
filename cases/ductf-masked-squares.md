# DownUnderCTF：从二进制恢复 flag 检查方程

[← 返回案例目录](../README.md) · 官方案例

- **作者 / 来源归属：** REA 官方案例团队；原项目作者见来源
- **核对日期：** 2026-10-16
- **收录状态：** 已阅读公开来源，确认原文明确使用 REA；本仓库未独立复跑。
- **分析目标：** DownUnderCTF 2023 的 masked squares flag checker，stripped Linux ELF

## 想解决什么问题

没有符号和源码，如何找出输入校验逻辑？

## REA 具体做了什么

用 REA 搜索提示字符串和交叉引用，分析校验函数、读取掩码与目标表；将 26 条约束交给 Z3 求解，并用进程捕获检查原题程序。

## 公开成果

以下是来源作者报告的成果：

官方记录了正确候选输出 Correct! / exit 0、错误候选输出 Incorrect! / exit 255；求解后再对照主办方源码与 metadata。

## 局限与未验证项

求解使用了常见 flag 格式和字符集假设；第二模型搜索超时，未证明唯一解。

## 可以借鉴什么

静态推理得到答案后，给原程序输入正确和错误样本，补上运行验证。

## REA 使用证据

原文中的定位摘录（Markdown 排版已简化；完整上下文以链接为准）：

> Fresh inspection and process captures on 8 October 2026, using the published REA 4.1.0 package

## 原始来源

- [公开原文 / 固定版本证据](https://github.com/morluto/rea/blob/42fc6c53ae188978deb3bedfe88287b6b316ba22/website/evidence/ctf-masked-squares.md)
- [项目 / 演示](https://rea.tools/showcase/ctf/)
- [补充来源 1](https://github.com/DownUnderCTF/Challenges_2023_Public/tree/b48f83db2984bc7fa2ec7879a32d7efb1be8d333/rev/masked-squares-flag-checker)

本页为独立中文整理，署名与成果归原作者。没有重新发布目标软件、安装包或完整反编译输出。
