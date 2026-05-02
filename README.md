# Problem Retrospect Skill

> 问题复盘技能 - 支持多种经典复盘方法论，生成向上汇报文档

## 支持的方法论

| 方法论 | 模式名称 | 适用场景 | 时间投入 |
|-------|---------|---------|---------|
| **丹纳赫5Why** | 标准模式 | 复杂问题、向上汇报 | 30-60min |
| **AAR** | 快速模式 | 任务回顾、小问题 | 15-30min |
| **A3** | 可视化报告 | 跨部门协调、归档 | 1-2h |

## 快速开始

### 安装

复制整个 `problem-retrospect-skill` 目录到您的 Claude Code skills 目录：

```bash
# macOS/Linux
cp -r problem-retrospect-skill ~/.claude/skills/

# Windows
copy problem-retrospect-skill C:\Users\[用户名]\.claude\skills\
```

### 使用

在 Claude Code 中直接说：

- 「做个复盘」 → 标准模式（丹纳赫5Why）
- 「用AAR做个快速复盘」 → AAR快速模式
- 「生成A3报告」 → A3可视化格式

## 技能结构

```
problem-retrospect-skill/
├── SKILL.md                    # 主技能文件
└── references/
    ├── danaher-framework.md    # 丹纳赫方法论详解
    ├── 5why-examples.md        # 5Why典型案例
    ├── aar-framework.md        # AAR事后回顾详解
    ├── a3-report-guide.md      # A3报告编写指南
    ├── report-template.md      # 向上汇报报告模板
    ├── improvement-sop-template.md  # 改进方案SOP模板
    └── methodology-comparison.md    # 12种方法论对比分析
```

## 核心流程

### 标准模式（丹纳赫5Why）

```
Phase 0: 入口分流 → 确定复盘类型和模式
Phase 1: 事实采集 → 4Agent并行采集（时间线/决策链/沟通/资源）
Phase 1.5: 检查点 → 用户确认事实完整性
Phase 2: 差距分析 → 量化目标与结果的差距
Phase 3: 根因深挖 → 5Why分析法挖到系统性根因
Phase 3.5: 检查点 → 用户确认根因深度
Phase 4: 方案制定 → 三维度改进方案（即时/机制/能力）
Phase 5: 报告生成 → 向上汇报文档
```

### AAR快速模式

```
Step 1: 预期什么？ → 建立预期基准
Step 2: 实际什么？ → 建立事实基础
Step 3: 为什么差异？ → 简化版根因分析
Step 4: 学到什么？ → 提取教训和行动
Step 5: 快速报告 → 简版复盘文档
```

## 输出文件

| 文件 | 内容 |
|------|------|
| `01-facts.md` | 时间线、决策链、沟通记录、资源变化 |
| `02-gap-analysis.md` | 差距分析表、差距类型分类 |
| `03-root-cause.md` | 5Why链条、根因分类、决策评估 |
| `04-improvements.md` | 改进方案三维度、SOP检查清单 |
| `复盘报告_完整版.md` | 向上汇报的完整复盘文档 |
| `A3报告.md` | 丰田一页纸可视化报告（可选） |

## 参考方法论

本技能整合了12种经典复盘方法论，详见 `references/methodology-comparison.md`：

- 丹纳赫5Why
- AAR（美军事后回顾）
- KPT
- Start/Stop/Continue
- Starfish
- PDCA
- A3（丰田一页纸）
- DMAIC（六西格玛）
- 8D
- ORID
- Toyota Kata
- Appreciative Inquiry

## 设计参考

- 女娲skill的流程结构和检查点设计
- gstack的完整性原则
- 丹纳赫的5Why根因分析法
- 美军AAR的快速复盘框架
- 丰田A3的一页纸可视化

## 许可证

MIT License

## 作者

Generated with Claude Code