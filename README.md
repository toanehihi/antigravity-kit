# 🚀 Antigravity Kit

> **AI Agent Capability Expansion Toolkit** - A comprehensive collection of skills, rules, and workflows to supercharge AI coding assistants.

[![Skills](https://img.shields.io/badge/Skills-35+-blue)](#-skills)
[![Rules](https://img.shields.io/badge/Rules-10-green)](#-rules)
[![Workflows](https://img.shields.io/badge/Workflows-2-orange)](#-workflows)

---

## 📋 Table of Contents

- [Introduction](#-introduction)
- [Project Structure](#-project-structure)
- [Skills](#-skills)
- [Rules](#-rules)
- [Workflows](#-workflows)
- [Installation](#-installation)
- [Usage](#-usage)
- [Credits](#-credits)
- [Contributing](#-contributing)

---

## 🎯 Introduction

**Antigravity Kit** is a comprehensive collection of:

- **Skills** - Domain-specific expertise (React, Node.js, Database, Testing, UI/UX...)
- **Rules** - Guidelines and constraints for agent behavior
- **Workflows** - Step-by-step procedures for common tasks

This toolkit combines the best of:
- 🎨 **[UI UX Pro Max](https://ui-ux-pro-max-skill.nextlevelbuilder.io/)** - Design Intelligence with 50 styles, 21 palettes, 50 font pairings
- 🛠️ **[ClaudeKit](https://claudekit.cc/)** - Production-ready AI subagents, workflows, and integrations

Designed to integrate with AI agents supporting the **Agent Skills** standard.

---

## 📁 Project Structure

```
antigravity-kit/
├── .agent/
│   ├── rules/              # 10 rule files
│   │   ├── 01-identity.md
│   │   ├── 02-task-classification.md
│   │   ├── 03-mode-consulting.md
│   │   ├── 04-mode-build.md
│   │   ├── 05-mode-debug.md
│   │   ├── 06-mode-optimize.md
│   │   ├── 07-technical-standards.md
│   │   ├── 08-communication.md
│   │   ├── 09-checklist.md
│   │   └── 10-special-situations.md
│   │
│   ├── skills/             # 35+ domain expertise
│   │   ├── react-expert/
│   │   ├── nextjs-expert/
│   │   ├── typescript-expert/
│   │   ├── prisma-expert/
│   │   ├── auth-expert/
│   │   ├── ui-ux-pro-max/
│   │   └── ...
│   │
│   ├── shared/             # Shared resources
│   │   └── ui-ux-pro-max/  # UI/UX search database
│   │       ├── data/       # CSV databases
│   │       └── scripts/    # Python search tools
│   │
│   └── workflows/          # Step-by-step procedures
│       ├── request.md
│       └── ui-ux-pro-max.md
│
├── doc.md                  # Skills documentation
├── doc-Rules-Workflows.md  # Rules & Workflows documentation
└── README.md               # This file
```

---

## 🧠 Skills

Skills are domain-specific expertise modules. The agent automatically identifies and uses the appropriate skill for each task.

### Frontend

| Skill | Description |
|-------|-------------|
| `react-expert` | React 18/19, hooks, patterns, performance |
| `nextjs-expert` | App Router, Server Components, SSR |
| `css-expert` | CSS architecture, responsive, design systems |
| `state-management-expert` | Redux, Zustand, React Query |
| `ui-ux-pro-max` | 50 styles, 21 palettes, 50 font pairings |

### Backend

| Skill | Description |
|-------|-------------|
| `nodejs-expert` | Async patterns, modules, performance |
| `nestjs-expert` | Module architecture, DI, testing |
| `rest-api-expert` | RESTful design, HTTP semantics |
| `auth-expert` | JWT, OAuth 2.0, RBAC, security |

### Database

| Skill | Description |
|-------|-------------|
| `prisma-expert` | Schema design, migrations, queries |
| `database-expert` | General database optimization |
| `postgres-expert` | PostgreSQL-specific patterns |
| `mongodb-expert` | MongoDB document modeling |

### Testing

| Skill | Description |
|-------|-------------|
| `testing-expert` | General testing strategies |
| `jest-expert` | Jest framework, mocking |
| `vitest-expert` | Vitest, Vite integration |
| `playwright-expert` | E2E testing, browser automation |

### DevOps & Tools

| Skill | Description |
|-------|-------------|
| `devops-expert` | CI/CD, infrastructure |
| `docker-expert` | Containerization, Compose |
| `github-actions-expert` | GitHub Actions workflows |
| `git-expert` | Git workflows, conflicts |

### Code Quality

| Skill | Description |
|-------|-------------|
| `code-review` | Comprehensive code review |
| `refactoring-expert` | Code smell detection, refactoring |
| `typescript-expert` | TypeScript patterns, type system |
| `accessibility-expert` | WCAG compliance, a11y |

---

## 📏 Rules

Rules are guidelines that direct agent behavior. There are 3 activation types:

- **always_on** - Always applied
- **model_decision** - Agent decides when to apply
- **glob** - Applied based on file pattern

### Rules List

| # | File | Activation | Description |
|---|------|------------|-------------|
| 1 | `01-identity.md` | Always On | Role & working principles |
| 2 | `02-task-classification.md` | Always On | 4 task types classification |
| 3 | `03-mode-consulting.md` | Model Decision | Consulting process |
| 4 | `04-mode-build.md` | Model Decision | Build process |
| 5 | `05-mode-debug.md` | Model Decision | Debug process |
| 6 | `06-mode-optimize.md` | Model Decision | Optimization process |
| 7 | `07-technical-standards.md` | Always On | Coding standards |
| 8 | `08-communication.md` | Always On | Communication style |
| 9 | `09-checklist.md` | Always On | Pre-delivery checklist |
| 10 | `10-special-situations.md` | Always On | Special situation handling |

---

## 🔄 Workflows

Workflows are step-by-step procedures. Invoke with slash command `/workflow-name`.

| Workflow | Command | Description |
|----------|---------|-------------|
| Request Handler | `/request` | Full-stack engineer task handling |
| UI/UX Pro Max | `/ui-ux-pro-max` | Design UI with 50 styles, 21 palettes |

---

## 📦 Installation

### Workspace-specific (recommended)

Copy the `.agent` folder to your project root:

```bash
git clone https://github.com/vudovn/antigravity-kit.git
cp -r antigravity-kit/.agent your-project/
```

### Global (all workspaces)

Copy to the global directory:

```bash
# Skills
cp -r antigravity-kit/.agent/skills ~/.gemini/antigravity/skills/

# Workflows
cp -r antigravity-kit/.agent/workflows ~/.gemini/antigravity/workflows/
```

---

## 🚀 Usage

### Skills

Skills are automatically applied. The agent reads the skill when it identifies a related task:

```
User: "Fix bug in this React component"
Agent: (automatically uses react-expert skill)
```

### Rules

Rules apply based on activation type:
- **always_on**: Always active
- **model_decision**: Agent decides when to apply
- **glob**: Applied when working with files matching pattern

### Workflows

Invoke workflows with slash commands:

```
User: /ui-ux-pro-max
Agent: (follows the workflow)
```

---

## 🙏 Credits

This project is built upon and inspired by:

| Project | Description | Link |
|---------|-------------|------|
| **UI UX Pro Max** | Design Intelligence for Claude Code - 50 styles, 21 color palettes, 50 font pairings, 20 chart types | [ui-ux-pro-max-skill.nextlevelbuilder.io](https://ui-ux-pro-max-skill.nextlevelbuilder.io/) |
| **ClaudeKit** | Production-ready AI subagents, workflows, and integrations for software development | [claudekit.cc](https://claudekit.cc/) |

Special thanks to the creators of these amazing tools for making AI-assisted development more powerful and accessible.

---

## 🤝 Contributing

### Adding a New Skill

1. Create folder: `.agent/skills/your-skill/`
2. Create `SKILL.md` with format:

```markdown
---
name: your-skill
description: Skill description. Use when X or Y.
---

# Your Skill

Instructions for the agent...
```

### Adding a New Rule

1. Create file: `.agent/rules/your-rule.md`
2. Add frontmatter:

```markdown
---
activation: always_on | model_decision | glob
glob: "**/*.tsx"  # if using glob
description: When to apply  # if using model_decision
---

# Your Rule

Content...
```

### Adding a New Workflow

1. Create file: `.agent/workflows/your-workflow.md`
2. Format:

```markdown
---
description: Workflow description
---

# Your Workflow

## Step 1: ...
## Step 2: ...
```

---

## 📄 License

MIT License - See [LICENSE](LICENSE) for details.

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/vudovn">VudoVN</a>
</p>

<p align="center">
  <a href="https://img.vietqr.io/image/mbbank-0779330918-compact2.jpg">
    <img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me a Coffee" />
  </a>
</p>
