# 版本记录

## v3.5.1 · 2026-10-22

- 新增英文版 `prompt-optimizer-en/`：由 v3.5.0 中文规则逐节翻译，规则不变；快捷写法中英文都认（如 `+explain` / `+讲解`）。
- 新增英文考卷 `evals/cases.en.json`（16 题，与中文考卷同编号、同考点，材料均为虚构）；`run_eval.py` 增加 `--lang en|zh`，默认仍跑中文。
- 新增 Claude Code 插件市场配置 `.claude-plugin/marketplace.json`，可一行命令安装中文版或英文版。
- 新增失败案例反馈表单（`.github/ISSUE_TEMPLATE/`）。
- README 改为英文首页，原中文 README 移到 `README.zh-CN.md`，内容保留并补充英文版、插件安装和反馈入口。
- 中文版 `SKILL.md`、`references/`、`agents/` 没有改动。英文版 16 题实测见 [VALIDATION.md](VALIDATION.md)。

## v3.5.0 · 2026-10-22

- 将经过单轮四题比较的 3.5-c3 提升为正式 3.5。仅调整候选版本标识并增加版本元数据，规则保持候选内容。
- 相比 3.4，集中更新保真原则、要求具体化和内部双向自检，减少无依据条件，同时保留明确方案设计任务中的方法补充。
- 替代此前 v3.5.0-beta.1；没有合入其额外工具流程规则。不同候选的历史成绩分别保留。
- 小范围比较观察到一题优化稿改善、三题持平，最终任务两版均四题合格。发布阶段不追加模型测试。
- v3.4.0 固定标签保存原公开主分支，提供回退；旧 beta 标签不移动。
- 2026-10-22 补充（文档更新，技能文件未改）：v3.4.0 与 v3.5.0 在 Claude 上同场跑完 16 题考卷并盲评，结果见 [VALIDATION.md](VALIDATION.md)。README 改为面向使用者的说明，原先的版本过程、v3.4.0 复测表和设计参考分别移到本文件、VALIDATION.md 和 [docs/design-references.md](docs/design-references.md)。

## v3.5.0-beta.1 · 2026-10-21（历史测试版）

侧重多轮授权与完成条件的另一份候选；已由正式 3.5.0 替代，内容与测试记录保留在原标签。

## v3.4.0（回退版本）

保留此前正式源文件和历史验证说明。具体记录见 [VALIDATION.md](VALIDATION.md) 与 [evals/README.md](evals/README.md)。
