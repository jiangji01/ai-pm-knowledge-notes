# ai-pm-knowledge-notes

适用于 **Cursor、Claude Code** 等支持 Agent Skills（单文件 `SKILL.md`）的环境：生成 **AI 产品经理应知应会**笔记时，统一采用 **① 知识本身｜② AI PM 内化｜③ 应用层实践** 三面结构。

## 仓库内容

```
ai-pm-knowledge-notes/
├── SKILL.md    # Skill 本体（必选）
├── README.md   # 安装说明（本文件）
├── LICENSE     # MIT
└── .gitignore
```

请复制 **`ai-pm-knowledge-notes` 整个目录**（不要只拷贝单个文件），否则会破坏各工具约定的路径层级。

## 安装

### Cursor（项目）

```text
<你的项目>/.cursor/skills/ai-pm-knowledge-notes/
```

### Claude Code（项目）

```text
<你的项目>/.claude/skills/ai-pm-knowledge-notes/SKILL.md
```

### Claude Code（个人）

```text
~/.claude/skills/ai-pm-knowledge-notes/SKILL.md
```

## 可选：默认产出路径

若 `SKILL.md`「落盘约定」中的默认文件夹与你的仓库结构不一致，在实施时请在对话里指定输出目录，或 fork 后在本地修改该表。

## 许可证

MIT，见 [LICENSE](LICENSE)。
