# Problem Retrospect Skill

> 问题复盘技能 - 支持3种经典方法论，生成向上汇报文档

[![License: MIT-0](https://img.shields.io/badge/License-MIT--0-green.svg)](https://opensource.org/licenses/MIT-0)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/zhilshi/problem-retrospect-skill)

---

## 📋 简介

采用丹纳赫方法论进行系统性问题复盘，支持三种模式：

| 方法论 | 模式 | 适用场景 | 时间 |
|-------|------|---------|------|
| **丹纳赫5Why** | 标准模式 | 复杂问题、向上汇报 | 30-60min |
| **AAR** | 快速模式 | 任务回顾、小问题 | 15-30min |
| **A3** | 可视化报告 | 跨部门协调、归档 | 1-2h |

---

## ✨ 核心特性

- ✅ **5阶段结构化流程** - 事实采集→差距分析→根因深挖→方案制定→报告生成
- ✅ **4Agent并行采集** - 时间线、决策链、沟通记录、资源变化
- ✅ **5Why根因深挖** - 穿透表象，挖到系统性根因
- ✅ **检查点确认** - Phase 1.5和3.5用户确认，确保质量
- ✅ **向上汇报文档** - 1500字简洁报告，适合上级阅读
- ✅ **A3一页纸报告** - 丰田可视化格式，跨部门协调
- ✅ **SOP检查清单** - 可执行的改进方案

---

## 🚀 快速开始

### 安装

```bash
# Clone仓库
git clone https://github.com/zhilshi/problem-retrospect-skill.git

# 复制到Claude Code skills目录
cp -r problem-retrospect-skill ~/.claude/skills/

# Windows用户
copy problem-retrospect-skill C:\Users\[用户名]\.claude\skills\
```

### 使用

在Claude Code中直接说：

```
做个复盘                    → 标准模式（丹纳赫5Why）
用AAR做个快速复盘           → AAR快速模式
生成A3报告                  → A3可视化格式
```

---

## 📖 使用示例

### 标准模式

```
用户：帮我做个复盘

AI：启动问题复盘技能...

Phase 0: 确定复盘类型和模式
Phase 1: 事实采集（4Agent并行）
  - 时间线：关键事件节点
  - 决策链：承诺背景和依据
  - 沟通记录：正式沟通频率
  - 资源变化：投入和约束变化

Phase 1.5: 事实确认检查点
→ 用户确认事实完整性

Phase 2: 差距分析（量化目标vs实际）
Phase 3: 根因深挖（5Why）

Why 1 → Why 2 → Why 3 → Why 4 → Why 5（系统性根因）

Phase 3.5: 根因确认检查点
→ 用户确认根因深度

Phase 4: 方案制定
  - 即时整改
  - 机制优化
  - 能力建设

Phase 5: 生成向上汇报报告
```

### AAR快速模式

```
用户：用AAR做个快速复盘

AI：启动AAR快速模式...

Step 1: 预期什么？ → 建立预期基准
Step 2: 实际什么？ → 建立事实基础
Step 3: 为什么差异？ → 简化根因分析
Step 4: 学到什么？ → 提取教训和行动
Step 5: 简版报告（500字以内）
```

---

## 📂 技能结构

```
problem-retrospect-skill/
├── SKILL.md                    # 主技能文件（23KB）
├── skill.json                  # 技能配置文件
├── LICENSE                     # MIT-0许可证
├── README.md                   # 说明文档
└── references/
    ├── danaher-framework.md    # 丹纳赫方法论详解
    ├── 5why-examples.md        # 5Why典型案例
    ├── aar-framework.md        # AAR事后回顾详解
    ├── a3-report-guide.md      # A3报告编写指南
    ├── report-template.md      # 向上汇报报告模板
    ├── improvement-sop-template.md  # 改进方案SOP模板
    └── methodology-comparison.md    # 12种方法论对比分析
```

---

## 📊 输出文件

| 文件 | 内容 |
|------|------|
| `01-facts.md` | 时间线、决策链、沟通记录、资源变化 |
| `02-gap-analysis.md` | 差距分析表、差距类型分类 |
| `03-root-cause.md` | 5Why链条、根因分类、决策评估 |
| `04-improvements.md` | 改进方案三维度、SOP检查清单 |
| `复盘报告_完整版.md` | 向上汇报的完整复盘文档 |
| `A3报告.md` | 丰田一页纸可视化报告（可选） |

---

## 🔧 支持的方法论

本技能整合了12种经典复盘方法论：

| 方法论 | 起源 | 本技能支持 |
|-------|------|-----------|
| 丹纳赫5Why | 丹纳赫公司 | ✅ 完整实现 |
| AAR | 美国陆军 | ✅ 完整实现 |
| A3 | 丰田汽车 | ✅ 完整实现 |
| KPT | 敏捷开发 | 📖 参考文档 |
| Start/Stop/Continue | 敏捷开发 | 📖 参考文档 |
| Starfish | Patrick Kua | 📖 参考文档 |
| PDCA | 戴明 | 📖 参考文档 |
| DMAIC | 六西格玛 | 📖 参考文档 |
| 8D | 福特汽车 | 📖 参考文档 |
| ORID | ICA | 📖 参考文档 |
| Toyota Kata | 丰田 | 📖 参考文档 |
| Appreciative Inquiry | Cooperrider | 📖 参考文档 |

---

## 📝 设计参考

- 女娲skill的流程结构和检查点设计
- gstack的完整性原则
- 丹纳赫的5Why根因分析法
- 美军AAR的快速复盘框架
- 丰田A3的一页纸可视化

---

## 📜 许可证

MIT-0 License (MIT No Attribution)

- ✅ Free to use, modify, and redistribute
- ✅ No attribution required
- ✅ Compatible with ClawHub publishing requirements

---

## 🤝 贡献

欢迎提交Issue和Pull Request！

---

## 📮 联系

- GitHub: https://github.com/zhilshi/problem-retrospect-skill
- Author: zhilshi

---

**版本**: 1.0.0
**更新日期**: 2026-05-02