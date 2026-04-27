# Skill Map

按“设计工作流 × 能力建设”的方式整理当前仓库规划。

## 工作流矩阵

| 阶段 | 目录 | 代表能力 | 当前状态 |
|------|------|---------|---------|
| 元能力 | `00-meta/` | 思考教练、系统思维、设计评审 | `thinking-coach`、`systems-design-advisor` 已实现 |
| 发现 | `01-discover/` | 用户研究、竞品分析、问题框定、对齐 | 规划中 |
| 定义 | `02-define/` | 信息架构、对象建模、旅程、流程、策略 | `object-modeling-for-design` 已实现 |
| 设计 | `03-design/` | 交互、UI、设计系统、响应式、原型 | 规划中 |
| 验证 | `04-validate/` | 可用性测试、启发式评估、无障碍 | 规划中 |
| 交付 | `05-deliver/` | handoff、review、文档 | 规划中 |
| 度量 | `06-measure/` | 埋点、实验、复盘 | 规划中 |
| 职业 | `07-career/` | 作品集、面试准备 | 规划中 |

## 当前落位

- `00-meta/thinking-coach/`
  - 当前承担思考教练 / 设计决策引导 / 复盘教练这条线
  - 适合作为整个仓库的元能力入口

- `00-meta/systems-design-advisor/`
  - 当前承担系统思维 / 系统化设计诊断这条线
  - 后续可以演进成计划里的 `systems-thinking`

- `02-define/object-modeling-for-design/`
  - 当前承担对象建模这条线
  - 后续可以继续补充 OOUX / enterprise patterns / 流程建模相关资源

## 优先级建议

建议先补齐以下方向：

1. `01-discover/user-research`
2. `01-discover/problem-framing`
3. `02-define/information-architecture`
4. `03-design/interaction-design`
5. `04-validate/usability-testing`
6. `00-meta/design-critique`

## 方法论来源

- `thinking-coach`：设计教练式提问、系统思维、结构化反思实践
- `systems-design-advisor`：Donella Meadows《系统之美》
- `object-modeling-for-design`：OOUX / Narrative Object Model / 企业后台对象建模实践
- 仓库整体规划：围绕“发现 -> 定义 -> 设计 -> 验证 -> 交付 -> 度量 -> 复盘/成长”的产品设计工作流

## 发布说明

- 源码按工作流阶段存放在 `00-meta/` 到 `07-career/`
- 可安装的 `.skill` 发布包统一放在 `packages/`
