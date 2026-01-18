# 🚀 Add Skill Installer

[![GitHub](https://img.shields.io/badge/GitHub-kevintsai1202-blue?logo=github)](https://github.com/kevintsai1202/add-skill-installer)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

透過 `npx add-skill` 從任何 Git 儲存庫安裝 Agent Skills 的技能指南。

## ✨ 功能特色

- 🔧 支援多種 Coding Agents
- 📦 從 GitHub、GitLab 或任何 Git URL 安裝技能
- 🌐 支援全域安裝或專案級安裝
- 🎯 可選擇安裝特定技能或全部技能

---

## 🤖 支援的 Agents

| Agent | 識別名稱 | 全域技能目錄 |
|-------|----------|--------------|
| **Antigravity** | `antigravity` | `~/.gemini/antigravity/skills/` |
| **Claude Code** | `claude-code` | `~/.claude/skills/` |
| **Cursor** | `cursor` | `.cursor/skills/` |
| **Codex** | `codex` | `.codex/skills/` |
| **OpenCode** | `opencode` | `.opencode/skills/` |
| **GitHub Copilot** | `github-copilot` | `.github/copilot/skills/` |
| **Roo Code** | `roo` | `.roo/skills/` |

---

## 📥 安裝此 Skill

### 全域安裝（推薦）

```bash
npx add-skill kevintsai1202/add-skill-installer -g -a antigravity -y
```

### 專案級安裝

```bash
npx add-skill kevintsai1202/add-skill-installer -a antigravity -y
```

---

## 🔧 CLI 完整用法

```
Usage: add-skill [options] <source>

Install skills onto coding agents (OpenCode, Claude Code, Codex, Cursor, Antigravity, Github Copilot, Roo Code)

Arguments:
  source                   Git repo URL, GitHub shorthand (owner/repo), or direct path to skill

Options:
  -V, --version            輸出版本號
  -g, --global             全域安裝（user-level）而非專案級
  -a, --agent <agents...>  指定目標 Agent
  -s, --skill <skills...>  指定要安裝的技能名稱
  -l, --list               列出儲存庫中可用的技能（不安裝）
  -y, --yes                跳過確認提示
  -h, --help               顯示說明
```

---

## 📚 來源格式範例

```bash
# GitHub 簡寫
npx add-skill vercel-labs/agent-skills

# 完整 GitHub URL
npx add-skill https://github.com/vercel-labs/agent-skills

# 指定特定路徑
npx add-skill https://github.com/vercel-labs/agent-skills/tree/main/skills/frontend-design

# GitLab URL
npx add-skill https://gitlab.com/org/repo

# SSH Git URL
npx add-skill git@github.com:vercel-labs/agent-skills.git
```

---

## ⚙️ 常用指令範例

### 列出可用技能

```bash
npx add-skill vercel-labs/agent-skills --list
```

### 安裝所有技能到 Antigravity（全域）

```bash
npx add-skill vercel-labs/agent-skills -g -a antigravity -y
```

### 安裝到多個 Agents

```bash
npx add-skill vercel-labs/agent-skills -g -a antigravity claude-code cursor -y
```

### 只安裝特定技能

```bash
npx add-skill vercel-labs/agent-skills --skill frontend-design -g -a antigravity -y
```

### 安裝多個特定技能

```bash
npx add-skill vercel-labs/agent-skills --skill frontend-design nextjs-expert -g -a antigravity -y
```

### 安裝到當前專案（非全域）

```bash
npx add-skill vercel-labs/agent-skills -a antigravity -y
```

### 互動式安裝（會提示選擇）

```bash
npx add-skill vercel-labs/agent-skills
```

---

## 🌟 推薦的技能儲存庫

| 來源 | 說明 |
|------|------|
| `vercel-labs/agent-skills` | Vercel 官方技能集 |
| [skillsmp.com](https://skillsmp.com/) | Skills Marketplace |
| [agentskills.io](https://agentskills.io/) | Agent Skills 社群 |

---

## 📋 前置需求

- Node.js 18+
- npm 或 pnpm

---

## 📄 授權

MIT License

---

## 🤝 貢獻

歡迎提交 Issue 和 Pull Request！
