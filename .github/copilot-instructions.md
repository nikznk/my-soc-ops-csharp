# Project Guidelines

## Code Style
- Use standard C# conventions: PascalCase for public types and members, camelCase for locals and private fields.
- Keep Blazor components focused on UI composition; keep game rules and state transitions in services.
- Follow existing utility-class styling patterns in SocOps/wwwroot/css/app.css.
- For frontend changes, follow these instruction files:
  - .github/instructions/css-utilities.instructions.md
  - .github/instructions/frontend-design.instructions.md

## Architecture
- App type: Blazor WebAssembly (.NET 10), bootstrapped in SocOps/Program.cs.
- Route entry point is SocOps/Pages/Home.razor, which switches between start and game states.
- Core boundaries:
  - UI components: SocOps/Components/
  - State orchestration and persistence: SocOps/Services/BingoGameService.cs
  - Bingo logic (board generation/checks): SocOps/Services/BingoLogicService.cs
  - Domain models: SocOps/Models/
  - Question data: SocOps/Data/Questions.cs
- State is persisted in browser localStorage through JS interop. Keep storage schema changes backward-compatible, or update version handling in BingoGameService.

## Build and Test
- From repository root:
  - Build: dotnet build SocOps/SocOps.csproj
  - Run: dotnet run --project SocOps/SocOps.csproj
- Prerequisite: .NET 10 SDK (see README.md).
- There is no dedicated test project in this workspace. If tests are added, include the test command in this file.

## Conventions
- Keep state updates event-driven via OnStateChanged in the game service, and dispose subscriptions in components/pages that subscribe.
- Prefer extending existing CSS utility classes over adding ad-hoc one-off styles.
- Keep docs concise and link to existing guides rather than duplicating:
  - README.md
  - workshop/GUIDE.md
  - CONTRIBUTING.md
