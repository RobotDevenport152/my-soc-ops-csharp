# Copilot Workspace Instructions

## ✅ Development Checklist (Before Commit)

- [ ] `dotnet build SocOps/SocOps.csproj` passes with no errors
- [ ] No compiler warnings
- [ ] Code follows C# naming conventions (PascalCase public, camelCase private)
- [ ] No unused imports or variables

## Quick Start

```bash
cd SocOps
dotnet build    # Build
dotnet run      # Dev server (http://localhost:5166)
```

## Project Overview

**Soc Ops** is a Blazor WebAssembly (.NET 10) Social Bingo game. Players find people matching questions to mark squares and achieve 5 in a row.

- 🎮 [Play](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
- 📚 [Lab Guide](workshop/GUIDE.md)
- 🔧 Tech: .NET 10, Blazor WASM, Custom CSS utilities

## Architecture

```
SocOps/
├── Components/      # Blazor components (BingoBoard, GameScreen, etc.)
├── Services/        # BingoGameService (state), BingoLogicService (rules)
├── Models/          # GameState, BingoSquareData, BingoLine
├── Pages/           # Home.razor (main entry)
├── Data/            # Questions.cs (bingo content)
└── wwwroot/         # Static assets & CSS utilities
```

**State Management**: Singleton `BingoGameService` with event-driven component updates. State persisted to localStorage.

**Styling**: Custom CSS utilities in `wwwroot/css/app.css` — see [CSS Guide](.github/instructions/css-utilities.instructions.md)

## Common Tasks

| Task | File(s) |
|------|---------|
| Add bingo questions | `Data/Questions.cs` |
| Modify game rules | `Services/BingoLogicService.cs` |
| Update component styling | `wwwroot/css/app.css` + utilities |
| New page | Add to `Pages/`, add route & nav link |

## Resources

- [CSS Utilities](.github/instructions/css-utilities.instructions.md)
- [Frontend Design Principles](.github/instructions/frontend-design.instructions.md)
- [Contributing Guide](CONTRIBUTING.md)
- Agents: `ui-review`, `tdd`, `quiz-master`, `pixel-jam` in `.github/agents/`

## Deployment

Auto-deploys to GitHub Pages on push to `main`.
