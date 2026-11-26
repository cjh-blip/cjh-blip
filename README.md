# cjh-blip

深圳技术大学 · 光源与照明 · 24 级。做光学仿真与照明计算的自动化。

## 在做什么

**光枢 / OptiFlow** —— 把 DXF 图纸送进 DIALux 做照明计算，全链路自动化。

```
图纸 → 房间/灯位识别 → 选灯 → 驱动 DIALux 落灯 → 实算 → 照度报告
```

三个仓分工：

| 仓 | 干什么 |
|---|---|
| [optiflow](https://github.com/cjh-blip/optiflow) | 平台层：IR、判据、五阶段工作流、报告 |
| [dialux-compiler](https://github.com/cjh-blip/dialux-compiler) | 驱动层：用 UIA 操作没有 API 的 DIALux |
| [dialux-furniture-catalog](https://github.com/cjh-blip/dialux-furniture-catalog) | 家具目录元数据清单（494 条家具 + 594 条 UI 条目） |

## 几条我认的规矩

- **不接受"看起来成功"**：预测值不写进实测字段，假状态一律堵死。
- **只决定放什么灯，不决定几盏灯**：灯位由图纸给定。
- **真机结论必须回流**：跑出来的结论变成代码默认值或测试，不停在手工链路里。

## 其他

- **[ParableHeart](https://github.com/cjh-blip/ParableHeart)** —— 把心理学论文里的抽象概念写成寓言故事。
- **[prompt-forge](https://github.com/cjh-blip/prompt-forge)** / **[plan](https://github.com/cjh-blip/plan)** / **[neat-freak](https://github.com/cjh-blip/neat-freak)** / **[standard-task-flow](https://github.com/cjh-blip/standard-task-flow)** —— 日常在用的 agent skills。
- **[3-provinces-6-ministries-agent](https://github.com/cjh-blip/3-provinces-6-ministries-agent)** —— 用三省六部制做多 agent 协同决策的玩具。

## 工具

Zemax · Python · PowerShell/UIA · DIALux evo · AutoCAD/DXF
