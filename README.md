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

在已 `git clone` 本仓库的机器上无需再做；本地从零发布可二选一。

### 方式 A：`gh` 一条命令（建库 + 推送）

```bash
brew install gh   # 尚未安装时
gh auth login     # 浏览器完成登录
cd ~/ai-pm-knowledge-notes
# 若已配置过 origin 且与目标一致，可直接 push；否则见方式 B
git push -u origin main
```

或直接让 `gh` 建库并推送（若本地 **没有** origin 时更干净）：

```bash
cd ~/ai-pm-knowledge-notes
git remote remove origin 2>/dev/null || true
gh repo create ai-pm-knowledge-notes --public --source=. --push
```

### 方式 B：网页建空库 + `git push`

1. 打开 [New repository](https://github.com/new)，名称填 **`ai-pm-knowledge-notes`**，**不要**勾选 README / .gitignore / license。  
2. 确认本地已：`git remote add origin https://github.com/<用户名>/ai-pm-knowledge-notes.git`  
3. `git push -u origin main`（HTTPS 首次会走系统凭据或浏览器登录）。

---

**维护者 [@jiangji01](https://github.com/jiangji01) 机器上**：仓库目录 `~/ai-pm-knowledge-notes` 已预设

`origin = https://github.com/jiangji01/ai-pm-knowledge-notes.git`

在网页创建 **同名空仓库** 后，于本机终端执行 `git push -u origin main` 即可完成闭环（CI/沙箱环境无法代你输入账号，需在你自己的终端完成一次认证）。

## 许可证

MIT，见 [LICENSE](LICENSE)。
