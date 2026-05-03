# ai-pm-knowledge-notes

适用于 **Cursor、Claude Code** 等支持 Agent Skills（`SKILL.md`）的工具：整理 **AI 产品经理应知应会**笔记时，固定 **① 知识本身｜② AI PM 内化｜③ 应用层实践**。

## 仓库内容

```
ai-pm-knowledge-notes/
├── SKILL.md    # Skill 本体（必选）
├── README.md   # 本说明
└── LICENSE     # MIT
```

安装时你需要的是 **整个文件夹**放入各工具的技能目录（见下），不要只散装一个文件导致路径报错。

## 安装

### Cursor（项目级）

```text
<你的项目>/.cursor/skills/ai-pm-knowledge-notes/
```

内含：`SKILL.md`（可复制本仓库整目录）。

### Claude Code（项目级）

```text
<你的项目>/.claude/skills/ai-pm-knowledge-notes/SKILL.md
```

### Claude Code（个人全局）

```text
~/.claude/skills/ai-pm-knowledge-notes/SKILL.md
```

## 默认输出路径

`SKILL.md` 中默认示例路径为 `ObsidianVault/AI产品应知应会/`。若无该目录，请在对话里指定输出文件夹，或 fork 后自行改 `SKILL.md` 第一节表格。

## 推送到 GitHub（首次）

在已 `git clone` 本仓库的机器上无需再做；若你在本地初始化：

1. 在 GitHub 网页 **New repository**，名称建议 `ai-pm-knowledge-notes`，**不要**勾选「Add README」（避免与本地冲突）。
2. 本地执行：

```bash
cd /path/to/ai-pm-knowledge-notes
git remote add origin https://github.com/<你的用户名>/ai-pm-knowledge-notes.git
git branch -M main
git push -u origin main
```

## 许可证

MIT，见 [LICENSE](LICENSE)。
