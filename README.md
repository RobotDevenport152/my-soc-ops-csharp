🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎯 Soc Ops

**The ultimate icebreaker for in-person mixers.** A fast-paced social bingo game that gets people talking, laughing, and connecting in real time.

Find people who match the questions. Mark your card. Get 5 in a row. **WIN.** 🎉

---

## 🚀 Get Started in Seconds

**Play online:**
> 👉 **[Launch the Game →](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)**

**Run locally:**
```bash
cd SocOps && dotnet run
```
Then open **http://localhost:5166** in your browser.

---

## 🎓 Learn Modern Web Development

This isn't just a game—it's a **full workshop** on building production-ready Blazor applications with AI assistance.

### 📚 Complete Lab Guide (5 Parts)

| 🎯 | Topic | What You'll Build |
|:---:|------|------------------|
| **00** | [Overview & Checklist](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Understand the project scope |
| **01** | [Setup & Context Engineering](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configure your workspace with Copilot |
| **02** | [Design-First Frontend](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Beautiful, responsive UI |
| **03** | [Custom Quiz Master](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Dynamic question generation |
| **04** | [Multi-Agent Development](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Orchestrate AI agents for complex tasks |

> 📖 **Prefer offline?** Read guides in [`workshop/`](workshop/) folder

---

## ⚡ What Makes It Special

✨ **Built with .NET 10** — Modern, performant Blazor WebAssembly
🎨 **Beautiful UI** — Responsive design with custom CSS utilities  
🧠 **Smart State Management** — Event-driven architecture with localStorage persistence
🤖 **AI-Ready** — Designed to be improved with Copilot at every step
🌍 **Real-Time** — Play anywhere, anytime with live game state

---

## 🛠️ Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

## 💻 Run It Your Way

### Local Development (Recommended for Learning)
```bash
git clone https://github.com/RobotDevenport152/my-soc-ops-csharp.git
cd my-soc-ops-csharp/SocOps
dotnet run
```

### GitHub Codespaces (Cloud IDE)
1. Click **Code** → **Codespaces** → **Create codespace on main**
2. Wait for setup (1-2 min)
3. In terminal: `cd SocOps && dotnet run`

### Build Only
```bash
cd SocOps
dotnet build
```

---

## 📁 Project Structure

```
├── Components/      # Blazor UI components (BingoBoard, GameScreen, etc.)
├── Services/        # Game logic & state management
├── Models/          # Data types (GameState, BingoSquareData, etc.)
├── Pages/           # Main page (Home.razor)
├── Data/            # Question library
└── wwwroot/         # CSS utilities & static assets
```

**State Flows Like This:**
```
User Click → BingoGameService → UpdateBoard → EmitEvent → ComponentsRerender
```

---

## 🎮 How to Play

1. **Tap "Start Game"** — Get your random bingo card
2. **Mingle & Match** — Ask people around you questions on your card
3. **Mark Squares** — Tap squares when you find someone who matches
4. **Get 5 in a Row** — Horizontal, vertical, or diagonal = **BINGO!**
5. **Celebrate** — You won! 🎊

---

## 🔧 Development

### Run Build & Tests
```bash
dotnet build SocOps/SocOps.csproj
```

### Linting
- Strict warnings-as-errors enabled
- Naming conventions enforced (PascalCase public, `_camelCase` private)
- Unused code detected automatically

See [Copilot Workspace Instructions](.github/copilot-instructions.md) for full details.

---

## 🎨 Customize

**Add New Questions:** Edit `SocOps/Data/Questions.cs`  
**Change Colors:** Modify CSS variables in `SocOps/wwwroot/css/app.css`  
**Adjust Game Rules:** Update `SocOps/Services/BingoLogicService.cs`

---

## 📚 Resources

- 🏗️ [Architecture & Development Guide](.github/copilot-instructions.md)
- 🎨 [CSS Utilities Reference](.github/instructions/css-utilities.instructions.md)
- 🤖 [Specialized Agents](.github/agents/) for TDD, UI review, design sprints
- 📖 [Contribution Guidelines](CONTRIBUTING.md)
- ⚖️ [License](LICENSE)

---

## 🤝 Contributing

We'd love your help! Check out [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:
- Code style (C# conventions, Blazor patterns)
- Pull request process
- Issue templates

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

**Ready to level up?** 👇

[▶️ Play Now](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) · [📚 Learn](workshop/GUIDE.md) · [🚀 Get Started](https://github.com/RobotDevenport152/my-soc-ops-csharp#-get-started-in-seconds)

</div>
