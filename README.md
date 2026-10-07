# UI Copy · 界面文案技能

面向网站、App、小程序和后台的 UI 文案编写与评审 skill。重点是让文字对应真实任务、状态和操作，帮助用户知道发生了什么、可以做什么、如何继续。

## 适用任务

- 写按钮、表单标签、辅助说明、空态、加载和成功反馈。
- 改善错误与恢复提示、删除确认、通知、分享标题和可访问名称。
- 删除重复提示，统一同一流程的术语，评审截图、设计稿或代码里的文案。

可只处理一个按钮，也可覆盖一条流程。通用原则跟随产品目标语言，另附中文表达参考；不绑定业务、框架、平台或外部服务。

## 使用示例

在 Codex 中可以显式使用 `$ui-copy`：

```text
用 $ui-copy 评审这个保存弹窗。只给文案建议，不改代码。
```

```text
用 $ui-copy 修改这个页面的空态和错误提示。
沿用现有术语，不改变交互；处理逻辑以提供的代码为准。
```

```text
用 $ui-copy 写三步表单的按钮文案，当前界面语言是英文。
提交后只保存草稿，还没有发布功能。
```

也可自然描述“检查这些按钮和错误提示是否清楚”。支持自动选择技能的工具会按描述判断是否使用；Claude Code 可使用 `/ui-copy`。传入当前文案、截图、设计稿或相关代码即可，不需要完整填写模板。

## 安装

下载或克隆本仓库，保持整个目录名为 `ui-copy`，将它放入所用工具的技能目录。`SKILL.md` 需直接位于 `ui-copy/` 下，不要多套一层；一起保留 `references/` 和 `agents/`。

| 工具 | 个人安装位置 | 项目安装位置 |
|---|---|---|
| Codex | `~/.agents/skills/ui-copy/` | `.agents/skills/ui-copy/` |
| Claude Code | `~/.claude/skills/ui-copy/` | `.claude/skills/ui-copy/` |

`~` 表示当前用户的主目录。自定义环境按其实际技能目录安装；不要在同一环境重复安装同名技能。其他支持 `SKILL.md` 的工具请遵循其技能发现方式。

位置与调用方式参见 [OpenAI Docs：Build skills](https://learn.chatgpt.com/docs/build-skills) 和 [Claude Code：Skills](https://code.claude.com/docs/en/skills)。安装与重新加载行为以所用版本为准；上述是格式和文档对应说明，尚未在所有工具中逐一运行验证。

本技能仅包含 Markdown 与 YAML，不需要 API Key、网络服务或安装运行依赖。参考链接在需要追溯指南或平台要求时查阅。

## 文件

| 文件 | 用途 |
|---|---|
| [SKILL.md](SKILL.md) | 触发范围、事实边界、写作方法和按风险选择的检查 |
| [references/patterns.md](references/patterns.md) | 组件细则、真实状态和成立条件明确的示例 |
| [references/zh-cn.md](references/zh-cn.md) | 中文语气、术语、数字、标点与动态文字 |
| [references/sources.md](references/sources.md) | 官方设计指南与参考范围 |
| [agents/openai.yaml](agents/openai.yaml) | Codex 界面显示名称与简短描述 |
| [LICENSE](LICENSE) | MIT 许可证 |

## 验证与贡献

修改时检查 YAML frontmatter、相对链接、触发范围，以及示例有没有承诺尚不存在的能力。评估实际使用效果时，保留页面状态、操作真实结果与判断依据；不要仅检查生成文案是否逐字等于示例。

欢迎补充具体问题、输入材料和可验证的行为前提。新增建议应帮助模型作出不同且更准确的判断，避免把单个产品习惯扩展成通用硬规则。

## 许可证

[MIT](LICENSE) · Copyright (c) 2026 UI Copy contributors。

许可适用于本仓库的技能说明、原创示例和配置。链接所指的第三方指南、品牌与资产不属于本仓库，不随本许可证重新授权。
