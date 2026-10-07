<p align="center">
  <img src="./assets/readme/hero.svg" width="100%" alt="UI Copy：让界面文字说清楚。打开文件选择器时，用“选择文件”表达动作，而不是提前宣告“上传完成”。">
</p>

# UI Copy

让 AI 写出的界面文字，对应**真实任务、状态和操作**。

面向网站、App、小程序和后台的文案技能。可以只改一个按钮，也可以评审一条流程；输入现有文案、截图、设计稿或相关代码即可。

[写作方法](SKILL.md) · [组件示例](references/patterns.md) · [中文表达](references/zh-cn.md) · [MIT](LICENSE)

## 先看三个例子

这些规范示例来自[组件与状态](references/patterns.md)。具体生成效果以实际使用与评测为准。

| 真实行为或状态 | 容易误导的文字 | 对应表达 |
|---|---|---|
| 只打开文件选择器 | 上传完成 | 选择文件 |
| 从列表移除，原文件保留 | 删除文件 | 移除文件 |
| 服务端提交结果未知 | 提交失败，请重试 | 暂未确认提交结果 |

**让用户少猜一步。** 恢复入口、撤销能力、权限和费用告知，都以产品的实际能力与必要信息为准。

## 它怎么判断

1. **这句话是否需要？** 删除重复解释，保留任务数据、操作后果和恢复信息。
2. **点击后立即发生什么？** 按钮表达真实动作；标题、选项和状态可以使用名词。
3. **事情进行到哪一步？** 区分提交中、已保存、已同步和结果未知，不提前宣告完成。

覆盖按钮、表单、空态、加载与成功反馈、错误、确认框、通知、分享标题和可访问名称。遵循产品的术语、品牌语气与目标语言，另附中文写作参考。

## 快速开始

以 Codex 个人安装为例，将仓库克隆到技能目录。

**macOS / Linux**

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/ZGY949/ui-copy.git ~/.agents/skills/ui-copy
```

**Windows PowerShell**

```powershell
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.agents\skills" | Out-Null
git clone https://github.com/ZGY949/ui-copy.git "$env:USERPROFILE\.agents\skills\ui-copy"
```

已安装时更新现有目录，避免重复安装同名技能。技能本体由 Markdown 与 YAML 构成，无需 API Key 或额外运行依赖。

然后给出一个明确的行为前提：

```text
用 $ui-copy 改写这个按钮：“上传完成”。
它点击后只打开文件选择器，还没有上传。
给出推荐文案和一句理由，不修改代码。
```

本规范对应的建议是“选择文件”：它描述点击后立即发生的动作。

<details>
<summary>其他工具与项目安装</summary>

| 工具 | 个人技能目录 | 项目技能目录 |
|---|---|---|
| Codex | `~/.agents/skills/ui-copy/` | `.agents/skills/ui-copy/` |
| Claude Code | `~/.claude/skills/ui-copy/` | `.claude/skills/ui-copy/` |

`~` 表示用户主目录。保留整个 `ui-copy` 目录，确保 `SKILL.md` 直接位于目录下。Claude Code 可用 `/ui-copy`；支持自动选择的工具也可按任务描述调用。

安装与重新加载方式以 [OpenAI Docs](https://learn.chatgpt.com/docs/build-skills) 和 [Claude Code 文档](https://code.claude.com/docs/en/skills)及所用版本为准。其他支持 `SKILL.md` 的工具按其发现机制安装；尚未逐一完成跨工具运行验证。

</details>

## 按你的任务使用

```text
用 $ui-copy 评审这个保存弹窗。只给文案建议，不改代码。
```

```text
用 $ui-copy 修改这个页面的空态和错误提示。
沿用现有术语，不改变交互；处理逻辑以提供的代码为准。
```

```text
用 $ui-copy 写三步表单的英文按钮文案。
提交后只保存草稿，还没有发布功能。
```

## 参考与贡献

[技能正文](SKILL.md)提供判断方法；[组件示例](references/patterns.md)和[中文表达](references/zh-cn.md)按需查阅。[参考来源](references/sources.md)说明对 Apple、IBM Carbon 和 Ant Design 官方指南的借鉴范围。

本技能约束表达，保留真实行为与必要告知。事实不足时给出成立条件；无法靠文案解决的交互问题单独指出。

欢迎提交具体问题、当前文案和真实行为前提。修改后检查引用与示例事实，评估实际生成结果；不只看文字是否逐字匹配示例。

## 许可证

[MIT](LICENSE) · Copyright (c) 2026 UI Copy contributors。许可适用于本仓库内容；链接中的第三方指南、品牌与资产不随本许可证重新授权。
