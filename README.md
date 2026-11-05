# 专业机械制图与 CAD 交付提示词

用于新建、修订和审查机械装配图、零件工作图与配套三维模型。以中文机械制图为主要场景，要求交付可编辑图纸，并把图线、剖切、尺寸、装配关系和原生文件检查落实到验收记录。

**直接调用**。打开 [PROMPT.md](PROMPT.md)，将全文交给 AI，再提供本次任务、基准版本和相关文件。需要复现减速器案例时，同时附上 [案例参数与修订记录](references/reducer-case.md)。在可读取仓库的工具里，也可以直接指向文件。

> 请读取本仓库的 PROMPT.md，并按其中的修订流程工作。以我标注的已批准 DWG 和对应三维装配为基准。只修订 A—A 剖视的轴承及螺钉中心线，另存新版。交付可编辑 DWG、同版 PDF 和核验结果。

**作为技能调用**。支持 Agent Skills 的环境可以加载本目录的 [SKILL.md](SKILL.md)，按该环境的文档注册 `mechanical-cad-drafting`。安装时保留目录结构。如果运行环境不能访问原生 CAD，仍可用主提示词审查图纸、整理参数并列出待验证项。 [Agent Skills 格式规范](https://agentskills.io/specification)

| 文件 | 内容 |
| --- | --- |
| [PROMPT.md](PROMPT.md) | 可单独复制的主提示词，含任务模板、绘图规则和发布验收清单 |
| [SKILL.md](SKILL.md) | Agent Skills 入口，按任务加载正文及可选案例 |
| [references/reducer-case.md](references/reducer-case.md) | 脱敏的同轴二级直齿减速器参数、修订决策和回归用例 |

案例数据来自一次课程设计，适合复现图样与测试提示词。用在其他项目时，以该项目的图样标准、工况、确认参数和交付要求为准。
