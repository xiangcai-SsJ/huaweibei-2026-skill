# 数学建模竞赛论文写作技能

本仓库提供一个可复用的 Codex 技能：[competition-modeling-paper](competition-modeling-paper/SKILL.md)。适用于国赛 CUMCM、美赛 MCM/ICM、华为杯和省级数学建模竞赛的完整论文写作与终稿审查。最终交付目标是一篇完整论文；技能先核对目标赛事的当年官方要求，再把赛题、模型、运行结果和检验串成可追溯的论证。

## 安装和调用

将 `competition-modeling-paper/` 整个文件夹复制到本机的 `$CODEX_HOME/skills/`（未设置时通常为 `~/.codex/skills/`），使 `SKILL.md` 位于该文件夹根目录。重新加载技能列表后，可在任务中写：

> 使用 `$competition-modeling-paper`，依据我提供的赛题、数据、最终结果和官方模板完成论文。

技能允许按描述自动匹配；仅把本仓库克隆到普通目录不会自动安装。需要复核时，提供赛题、原始数据、最终方案表、运行日志、现有稿件和赛事年度；资料不足时技能会先给出简短的对齐块，最多询问三个必须澄清的问题。

## 目录

```text
competition-modeling-paper/
├── SKILL.md                          核心工作流与结论边界
├── agents/openai.yaml                技能列表显示信息
└── references/
    ├── paper-structure.md            各章节要点、篇幅与常见错误
    ├── quality-gates.md              成稿前、成稿后的双轮体检
    └── huawei-2026-d-case.md         2026 华为杯 D 题案例证据地图
```

案例参考链接到[2026 华为杯 D 题项目归档](https://github.com/xiangcai-SsJ/huaweibei-2026)，并明确标注其审查尚未关闭的事项。案例数值只用于定位对应方案版本，使用时须重新核对最新文件与当届官方规定。
