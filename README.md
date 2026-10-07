<p align="center">
  <img src="./assets/readme/hero.svg" width="100%" alt="UI Copy：减少 AI 页面中的说明文字。把一段解释筛选方式的文字，变成项目列表旁的状态筛选控件。">
</p>

# UI Copy

**减少 AI 页面里的冗长说明，把必要信息放回界面。**

AI 做页面时，常用长段文字介绍功能、解释操作、填满空态。UI Copy 帮你决定这些文字该删、该缩、该放在哪里，以及哪些更适合由交互表达，让页面简洁、清楚、精致。

[技能正文](SKILL.md) · [处理示例](references/patterns.md) · [中文表达](references/zh-cn.md) · [MIT](LICENSE)

## 它解决这样的页面问题

### 一个短语就够

> 在这里，你可以查看和管理自己创建的所有项目。

改为标题 **“我的项目”**，下方直接展示列表。标题和内容已经表达的事，不再重复介绍。

### 解释变成直接操作

> 你可以根据项目状态筛选列表，查看正在进行或已经完成的项目。

在列表附近提供 **“全部／进行中／已完成”** 筛选项。选择后实际更新列表，控件本身表达怎么用。

页面实现范围明确、状态数据已可用时，落实筛选行为；只做评审时给出具体交互建议。首图是呈现示意，具体页面中的交互需要实现并验证。

### 必要信息放对位置

把“请在下方输入项目名称……”改为字段标签 **“项目名称”**。格式或限制需要提前知道时，就地提供短提示；少见的补充帮助可按需展开。

## 四种处理

- **删重复**：去掉标题、控件和状态已表达的介绍。
- **缩表达**：长句变成清楚的词或短语。
- **放对位**：信息回到标题、标签、状态、提示或详情。
- **转交互**：用真实的搜索、筛选、切换、添加等操作承接解释。

保留任务数据、必要告知和恢复信息。简洁应让用户更容易理解与操作，不能靠隐藏关键条件、难发现的图标或空有外观的按钮。

## 快速开始

以 Codex 个人安装为例：

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

```text
用 $ui-copy 精简这个项目列表页。
减少解释性段落，整理必要信息的位置。
列表已有状态数据，把筛选说明改成可用的状态筛选。
保留原业务规则和必要告知。
```

<details>
<summary>其他工具与安装位置</summary>

| 工具 | 个人技能目录 | 项目技能目录 |
|---|---|---|
| Codex | `~/.agents/skills/ui-copy/` | `.agents/skills/ui-copy/` |
| Claude Code | `~/.claude/skills/ui-copy/` | `.claude/skills/ui-copy/` |

`~` 表示用户主目录。保留完整的 `ui-copy` 目录，确保 `SKILL.md` 位于目录下。Claude Code 可用 `/ui-copy`；支持自动选择的工具也可按任务描述调用。

安装方式以 [OpenAI Docs](https://learn.chatgpt.com/docs/build-skills) 和 [Claude Code 文档](https://code.claude.com/docs/en/skills)及所用版本为准。其他支持 `SKILL.md` 的工具按其发现机制安装；尚未逐一完成跨工具运行验证。

</details>

## 适用范围与贡献

用于制作、修改或评审网站、App、小程序和后台页面。只读评审、文案修改与页面实现分别遵循各自授权范围；涉及新业务规则、外部服务或费用时按项目边界处理。

文章、知识正文和用户内容按其内容目标保留。少见的帮助可以按需出现，影响决定的关键条件仍须就地可见。

欢迎提供有冗长说明的页面、实际任务与行为前提。参考依据见[来源说明](references/sources.md)。

## 许可证

[MIT](LICENSE) · Copyright (c) 2026 UI Copy contributors。链接中的第三方指南、品牌与资产不随本许可证重新授权。
