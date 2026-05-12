🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎲 Soc Ops

**Social Bingo for in-person mixers — powered by Blazor & GitHub Copilot Agent Mode**

Find people who match the questions. Get 5 in a row. Break the ice! 🧊

[![.NET 10](https://img.shields.io/badge/.NET-10-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor WebAssembly](https://img.shields.io/badge/Blazor-WebAssembly-512BD4?logo=blazor&logoColor=white)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![GitHub Pages](https://img.shields.io/badge/Deployed-GitHub%20Pages-222?logo=github&logoColor=white)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
[![GitHub Copilot](https://img.shields.io/badge/Built%20with-GitHub%20Copilot-000?logo=githubcopilot&logoColor=white)](https://github.com/features/copilot)

[🎮 **Play the Game**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) &nbsp;•&nbsp; [📚 **Lab Guide**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) &nbsp;•&nbsp; [⚡ **Quick Start**](#-quick-start)

</div>

---

## ✨ What Is This?

**Soc Ops** is two things in one:

| | |
|---|---|
| 🎮 **A Social Bingo game** | An interactive icebreaker for meetups, workshops, and team events. Players roam the room finding people who match fun prompts on their bingo card. |
| 🧑‍💻 **A hands-on Copilot lab** | A structured workshop where you use **VS Code Agent Mode** to redesign the UI, generate quiz content, and build new features — all guided by AI. |

You start with a working app and leave with a custom-themed bingo game *and* real-world AI-assisted development skills.

---

## 🎯 What You'll Learn

| # | Skill | Description |
|---|-------|-------------|
| 1 | **Context Engineering** | Teach Copilot about your codebase with `.github/instructions` files |
| 2 | **Agentic Workflows** | Use background agents, cloud agents, and custom agent modes |
| 3 | **Design-First Development** | Let AI iterate on UI themes while you steer the creative vision |
| 4 | **Test-Driven Development** | Use TDD agents (Red → Green → Refactor) for reliable feature builds |

---

## 📚 Lab Guide

> ⏱️ ~1 hour &nbsp;|&nbsp; 🎓 Intermediate &nbsp;|&nbsp; 🛠️ C# / .NET 10 / Blazor WebAssembly

| Part | Title | Time |
|------|-------|------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview & Checklist | — |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup & Context Engineering | 15 min |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend | 15 min |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master | 10 min |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development | 20 min |

> 📝 Prefer offline reading? Lab guides are also available in the [`workshop/`](workshop/) folder.

---

## ⚡ Quick Start

### Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher
- [VS Code](https://code.visualstudio.com/) with **GitHub Copilot** (Pro / Business / Enterprise)

### Option A — GitHub Codespaces ☁️ *(fastest)*

1. Click **Use this template** to create your own repo
2. Open your repo → **Code** → **Codespaces** → **Create codespace on main**
3. Wait for the devcontainer to finish setup, then run:
   ```bash
   cd SocOps && dotnet run
   ```

### Option B — Local Development 💻

```bash
# Clone your repo and run
cd SocOps
dotnet run
```

The app will open at `http://localhost:5000`. Deploys automatically to **GitHub Pages** on every push to `main`.

---

## 🗂️ Project Structure

```
SocOps/
├── Components/          # Reusable UI components
├── Data/Questions.cs    # Bingo prompts — customize these!
├── Pages/Home.razor     # Main game page
├── Services/            # Game logic & state
└── wwwroot/css/app.css  # Utility classes (Tailwind-style)
```

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

<div align="center">

Made with ❤️ for developer communities &nbsp;•&nbsp; [Code of Conduct](CODE_OF_CONDUCT.md) &nbsp;•&nbsp; [License](LICENSE)

</div>
