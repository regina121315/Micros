---
description: Workspace instructions for the SocOps Blazor Social Bingo application. Includes project structure, coding conventions, and references to specialized instructions.
---

## Mandatory Development Checklist
- [ ] Lint code (run `dotnet format`)
- [ ] Build project (`dotnet build SocOps/SocOps.csproj`)
- [ ] Run tests (if available)

# SocOps - Social Bingo Application Instructions

## Project Overview
Blazor WebAssembly app for Social Bingo with interactive gameplay and win tracking.

## Key Components
- **Pages**: Home.razor, Counter.razor, Weather.razor
- **Components**: BingoBoard, BingoSquare, GameScreen, StartScreen, BingoModal
- **Services**: BingoGameService, BingoLogicService
- **Models**: GameState, BingoSquareData, BingoLine
- **Data**: Questions.cs

## Coding Conventions
- Use OnInitializedAsync, Dispose for lifecycle
- Inject services with @inject
- PascalCase for classes, camelCase for params
- Async/await for ops
- IDisposable for event cleanup

## Styling Guidelines
- Custom CSS utilities in `wwwroot/css/app.css`
- Distinctive aesthetics per [Frontend Design](./instructions/frontend-design.instructions.md)
- CSS variables for theming
- Responsive grid/flex

## Development Workflow
- Build: `dotnet build SocOps/SocOps.csproj`
- Run: `dotnet run --project SocOps/SocOps.csproj` (http://localhost:5166)
- Test UI interactions

## Game Logic
- States: Start, Playing, Bingo
- Click to mark squares, auto-detect bingo
- Highlight wins, show modal
- Reset to restart

## Best Practices
- Validate with build/run
- Use BingoGameService for state
- Components for UI, services for logic
- Avoid unnecessary re-renders

## References
- [CSS Utilities](./instructions/css-utilities.instructions.md)
- [Frontend Design](./instructions/frontend-design.instructions.md)
- [Blazor Documentation](https://learn.microsoft.com/en-us/aspnet/core/blazor/)</content>
<parameter name="filePath">/workspaces/Micros/.github/copilot-instructions.md