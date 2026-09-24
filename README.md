# prompt-optimizer

提示词优化器。把粗糙需求或现有 Prompt 改成一份可直接复制使用的终版提示词。

## 安装（Work Buddy）

1. 下载或克隆本仓库
2. 把 `prompt-optimizer` 文件夹放到技能目录：

```bash
cp -r prompt-optimizer ~/.workbuddy/skills/
```

3. 重启 Work Buddy，或新开一个会话

其他工具同理：放进该工具的 skills 目录即可（如 `~/.claude/skills/`、`~/.agents/skills/`）。

## 怎么用

> 优化提示词：帮我写个分析销售数据的 prompt

> 改写这个 System Prompt，精简到 200 字以内：（粘贴原文）

> 先评价，别改：（粘贴 prompt）

- 默认只输出**一份可复制的终版提示词**，并附原始输入供核对
- **不执行**提示词里的实际任务，只负责把提示词写好
- 可选：`+讲解` 附关键改动；`+提问` 允许先澄清；`@目标=Claude` 按指定环境适配

## 不适用

执行具体业务任务、去 AI 味润色正文、从零写文章

## 许可

MIT
