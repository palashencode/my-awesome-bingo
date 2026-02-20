# Copilot Instructions for My Awesome Bingo

## Development Checklist
- [ ] Lint: `npm run lint`
- [ ] Build: `npm run build`
- [ ] Test: `npm run test`

## Architecture
React TypeScript app with Vite & Tailwind v4. State in `useBingoGame` hook (localStorage persisted). Game logic in `utils/bingoLogic.ts` (5x5 grid). Data in `data/questions.ts`.

## Key Patterns
- State auto-saves with version validation
- Bingo checks after square toggles via `checkBingo()`
- Board shuffles 24 questions + center free space (index 12)
- Props pass data down (e.g., `board`, `winningSquareIds`)

## Workflows
- Dev: `npm run dev`
- Build: `npm run build`
- Test: `npm run test`
- Lint: `npm run lint`

## Styling
Tailwind v4 with `@theme` in `index.css` for custom colors. Use `bg-marked`, `border-marked-border`. Avoid generic aesthetics per `frontend-design.instructions.md`. Responsive grids with `grid-cols-5`.

## Testing
Vitest with `@testing-library/react`. Mock Math.random with `vi.spyOn()`. Test utils functions and component behavior.

## Examples
- Add question: Update `questions` in `data/questions.ts`
- New state: Add to `GameState` type, handle in `useBingoGame`
- Style: Conditional classes like `isMarked ? 'bg-marked' : 'bg-white'`</content>
<parameter name="filePath">c:\_WS\CopilotSession\my-awesome-bingo\.github\copilot-instructions.md