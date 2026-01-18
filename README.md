# 🚀 Add Skill Installer

[![GitHub](https://img.shields.io/badge/GitHub-kevintsai1202-blue?logo=github)](https://github.com/kevintsai1202/add-skill-installer)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

透過 `npx add-skill` 從任何 Git 儲存庫安裝 Agent Skills 的技能指南。

## ✨ 功能特色

- 🔧 支援多種 Coding Agents（Antigravity、Claude Code、Cursor 等）
- 📦 從 GitHub、GitLab 或任何 Git URL 安裝技能
- 🌐 支援全域安裝或專案級安裝
- 🎯 可選擇安裝特定技能或全部技能

## 🤖 支援的 Agents

| Agent | 技能目錄 |
|-------|----------|
| **Antigravity** | `~/.gemini/antigravity/skills/` |
| Claude Code | `~/.claude/skills/` |
| Cursor | `.cursor/skills/` |
| Codex | `.codex/skills/` |

## 📥 安裝方式

### 作為全域技能安裝此 Skill

```bash
npx add-skill kevintsai1202/add-skill-installer -g -a antigravity -y
```

### 安裝到當前專案

```bash
npx add-skill kevintsai1202/add-skill-installer -a antigravity -y
```

## 🔧 使用方式

安裝完成後，只需告訴 Agent：

> 「幫我安裝 vercel-labs/agent-skills 的技能」

Agent 會自動觸發此技能並引導你完成安裝流程。

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
```

## ⚙️ 常用選項

| 選項 | 說明 |
|------|------|
| `-g, --global` | 安裝到全域目錄（跨專案可用） |
| `-a, --agent <agents...>` | 指定目標 Agent |
| `-s, --skill <skills...>` | 只安裝特定技能 |
| `-l, --list` | 列出儲存庫中可用的技能 |
| `-y, --yes` | 非互動式安裝 |

## 🌟 推薦的技能儲存庫

- **Vercel Labs**: `vercel-labs/agent-skills`
- **Skills Marketplace**: [skillsmp.com](https://skillsmp.com/)
- **Agent Skills**: [agentskills.io](https://agentskills.io/)

## 📋 前置需求

- Node.js 18+
- npm 或 pnpm

## 📄 授權

MIT License

## 🤝 貢獻

歡迎提交 Issue 和 Pull Request！
