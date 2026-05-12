# Project Guidelines

## Mandatory Development Checklist
Complete all items before finalizing changes:
- [ ] Lint: `dotnet format --verify-no-changes SocOps/SocOps.csproj`
- [ ] Build: `dotnet build SocOps/SocOps.csproj`
- [ ] Test: `dotnet test`

## Architecture
- Blazor WebAssembly (.NET 10) app bootstraps in SocOps/Program.cs.
- Main route/page is SocOps/Pages/Home.razor.
- UI lives in SocOps/Components/.
- State and persistence logic belong in SocOps/Services/BingoGameService.cs.
- Bingo rules/board logic belong in SocOps/Services/BingoLogicService.cs.
- Question content lives in SocOps/Data/Questions.cs.

## Code and Styling Conventions
- Keep components UI-focused; keep behavior in services.
- Use standard C# naming conventions.
- Reuse utility classes from SocOps/wwwroot/css/app.css before adding one-off styles.
- Follow:
  - .github/instructions/css-utilities.instructions.md
  - .github/instructions/frontend-design.instructions.md

## Build and Run
- Prerequisite: .NET 10 SDK (README.md).
- Run locally: `dotnet run --project SocOps/SocOps.csproj`

## Docs
Link to existing docs instead of duplicating:
- README.md
- workshop/GUIDE.md
- CONTRIBUTING.md
