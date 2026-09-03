# Skills

这些 skill 来自 [mattpocock/skills](https://github.com/mattpocock/skills)（Matt Pocock，MIT 许可，
许可正文见 `LICENSE.mattpocock-skills`）。装在仓库里，Claude Code 的云端 / 本地 / IDE 会话都会自动加载。

- 安装版本：plugin `mattpocock-skills` v1.2.3，上游 commit `6654f6b`
- 安装范围：上游 `skills/engineering/` + `skills/productivity/`（即插件清单里的 25 个），
  目录已铺平为 `.claude/skills/<name>/`；`in-progress/`、`misc/`、`deprecated/` 未安装
- Codex 专用的 `agents/openai.yaml` 已移除，只保留 Claude Code 需要的部分

## 常用入口

| 命令 | 用途 |
| --- | --- |
| `/grill-me`、`/grill-with-docs` | 动手前先让 agent 反问你，把需求问清楚 |
| `/to-spec`、`/to-tickets` | 把对话结果落成 spec / 工单 |
| `/tdd`、`/implement` | 测试先行地实现 |
| `/code-review`、`/diagnosing-bugs` | 审查代码、定位 bug |
| `/triage`、`/wayfinder`、`/handoff` | 分类 issue、在陌生代码里找路、交接上下文 |

首次使用建议先跑一次 `/setup-matt-pocock-skills`：它会问你用哪个 issue tracker、triage 用什么标签、
文档放哪里，并把答案写进仓库配置。

## 更新

重新从上游拷贝即可（保持同样的铺平结构），或改用官方插件：`/plugin install mattpocock-skills`
（插件是托管只读版，会自动更新；两种方式只选一种，否则每个 skill 会出现两份）。
