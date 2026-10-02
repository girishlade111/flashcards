# flashcards

A React flashcard study component (`LlamaFlashcards`) — an interactive flashcard deck with front/back cards for self-testing. Built as a single self-contained component using React hooks (`useState`) and shadcn/ui primitives (`Button`, `Card`, `Input`, `Label`).

## ✨ Features

- **Flip-style flashcard deck** — click a card to reveal the answer on the back.
- **Pre-loaded llama trivia set** — 5 sample cards (family, lifespan, origin, babies, group name) to demonstrate the format.
- **Editable deck** — add your own front/back pairs via the included input controls.
- **TypeScript types** — a `Flashcard` type (`front`, `back`) for type-safe cards.

## 🛠️ Tech Stack

- React 18+ (hooks: `useState`)
- TypeScript
- shadcn/ui components (`button`, `card`, `input`, `label`)
- Tailwind CSS (styling via shadcn classes)

## 🚀 Quick Start

The repo ships a single component file (`flashcards`) intended to be dropped into an existing React + shadcn/ui project.

1. Install shadcn/ui components (if not present):
   ```bash
   npx shadcn@latest add button card input label
   ```
2. Rename the component file to `LlamaFlashcards.tsx` and place it under your components directory, e.g. `components/LlamaFlashcards.tsx`.
3. Fix the import paths (the snippet uses absolute paths like `"/components/ui/button"` — change to `@/components/ui/button` or the correct relative path).
4. Import and render it in a page/route:
   ```tsx
   import LlamaFlashcards from "@/components/LlamaFlashcards";

   export default function StudyPage() {
     return <LlamaFlashcards />;
   }
   ```

## 📁 Project Structure

| File | Purpose |
|---|---|
| `flashcards` | The React flashcard component (TypeScript/JSX) |
| `README.md` | This file |
| `LICENSE` | License |

## ⚠️ Notes

- The component references `LlamaFlashcards` as its default export but the deck contents are fully editable — replace the `initialFlashcards` array with your own study set.
- This is a **component snippet, not a standalone app** — it needs a host React project with shadcn/ui installed to run. It is not deployed as a website.

## 👤 Author

*Built by Girish Lade — [ladestack.in](https://ladestack.in)*

## 📄 License

See [LICENSE](LICENSE).
