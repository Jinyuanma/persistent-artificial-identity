# Persistent Artificial Identity

**Persistent, Developing Artificial Individuality** — 研究具有长期记忆、发展过程和持续个体差异的人工系统。

项目启动：2026-10-31 · 阶段：研究定义与架构探索 · 状态：尚无可运行原型或实验结果。

## 核心问题

> 同一个基础模型，能否仅因不同的经历，逐渐形成稳定、可测量且持续发展的个体差异？

本项目从动态的 **Computational Person Model** 出发：

```text
Artificial Individual
  = Base Model + Identity State + Memory + Development Process

Person(t+1) = F(Person(t), Experience(t))
```

目标是研究长期发展的身份结构。静态 persona prompt 可以作为实验基线，但不是项目的最终系统。

## 拟研究的内部结构

| 结构 | 研究内容 |
| --- | --- |
| Traits | 相对稳定的行为倾向及缓慢变化机制 |
| Goals / Values / Beliefs | 目标、价值、信念、证据与置信度 |
| Memory | 情节记忆、语义记忆、个人语义记忆 |
| Self-model | 系统对自己的认识，与实际内部状态分别表示 |
| Narrative | 对经历的解释、意义组织与身份叙事 |
| Relationships | 面向不同对象的关系、信任及相关经历 |
| Current state | 情境、情绪类状态、精力、压力及注意力的计算表征 |

拟议闭环：

```text
Experience → Memory → Reflection / Consolidation
                           ↓
              Beliefs / Goals / Relationships
                           ↓
                  Self-model / Narrative
                           ↓
                    Action → Experience
```

上述分层和更新路径都是待检验的设计假设。慢变量和快变量应有不同更新规则；单次外部评价应作为带来源的观察记录，不直接覆写身份。

## 项目记录

- [完整原始构想（中文）](docs/ORIGINAL_VISION.zh-CN.md)：保留项目起点及全部 17 节讨论。
- [研究任务书](docs/PROJECT_CHARTER.zh-CN.md)：范围、原则、关键问题和完成标准。
- [研究路线图](docs/ROADMAP.zh-CN.md)：从定义到最小原型，再到受控实验。

下一步：先明确 v0.1 数据结构、状态更新契约与评估协议，再实现最小闭环。

## 研究边界

本项目中的 identity、self、mood 等词指可实现和可测量的计算表征。个体差异、心理学映射及身份持续性均需实验支持；本仓库不声称系统具有意识、主观体验或人格权。原始构想中的理论名称、变量和时间尺度需经后续文献核验，不作为已验证结论。

公开仓库的初期实验使用合成经历；真实私人对话和身份数据不作为默认公开材料。
