# FPGA 系统设计与 DSP 实时信号处理学习仓库

以任务驱动、可中断恢复的方式训练独立工程能力，重点为 DSP 建模、定点化、FPGA 实时部署和系统设计。核心学习代码由用户编写，AI 提供讲解、提示、评审和工程咨询。

## 从哪里继续

- [当前进度与恢复点](management/CURRENT.md)：每次恢复先读这里。
- [长期 Agent 规则](AGENTS.md)：教学边界、操作授权与成果保护。
- [自主学习工作流](WORKFLOW.md)：继续、选题、暂停、评审与验收流程。
- [路线与依赖](management/ROADMAP.md)、[任务索引与模板](management/TASKS.md)。
- [能力画像](management/SKILLS.md)、[重要决策](management/DECISIONS.md)。
- [厂家资料索引](docs/references/BX71.md)、[BX71 硬件核验](hardware/BX71/README.md)。

可直接提出“继续上次学习”“推荐下一项任务”“我想学习某知识点”“暂停当前任务”“恢复某任务”或“复盘知识盲区”。可选择独立练习、提示、详细讲解、代码评审；不设每日任务量与固定课程日程。

## 平台与现状

工作目录：`D:\Users\Admin\Desktop\agent_wp\fpga-dsp-lab`。

训练平台为 BX71 Zynq-7020，Vivado 2020.2，MATLAB/Python；后续按需使用 HDL Coder。文件证据标注 XC7Z020-2CLG400I，PL 时钟 50 MHz/U18。实物版本、IO 调压归属、DDR 参数与扩展模块仍需核对，详见硬件记录。

已完成本地最小文档初始化、资料索引及 [M0 诊断准备](diagnostics/README.md)；四项诊断均待用户选择开始。Python/Git 版本查询已成功，Vivado 与 MATLAB 的工程运行能力尚未验证。云端仓库为 [hahax1ao/fpga-dsp-lab](https://github.com/hahax1ao/fpga-dsp-lab)，用户明确选择保持公开。已配置 origin；实际同步状态以 Git 与 CURRENT 中的核验记录为准。

## 按需扩展目录

当前实际使用 `management/`、`docs/references/`、`hardware/BX71/`、`diagnostics/`。后续出现任务时才创建 `exercises/`、`labs/`、`projects/`；`tools/` 仅存放经批准的辅助工具。

任务说明与该任务源码、TB、模型、约束、结果集中保存，不散落在公共目录。手写 HDL 与专业工具生成 HDL 分开管理，记录生成参数、版本和复现过程。厂家原件留在 E 盘，不整体纳入 Git。

## Git 使用

本地仓库使用 main，小练习可直接在 main 工作；复杂任务按确认后的方案使用任务分支。每次提交、推送、合并都需用户确认。`.gitignore` 仅过滤典型缓存和 Vivado 运行产物，保留 XDC、IP 配置、报告及原始结果。提交前必须检查实际待提交文件，忽略规则不能替代审查。
