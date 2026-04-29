# pi-prompt-shelf

A [Pi](https://github.com/nicholasgasior/pi-coding-agent) extension that lets you stash prompts from the editor into a persistent shelf instead of submitting them. Shelved prompts survive across sessions and are always visible as a widget above the editor input.

## Features

- **Persistent shelf** — prompts are saved to `~/.pi/agent/prompt-shelf.json` and persist across sessions
- **Widget display** — a bordered widget above the editor shows all shelved prompts with timestamps
- **Quick restore** — restore any prompt by number with `Alt+1..9`
- **Interactive picker** — browse, restore, or delete shelved prompts with the `/shelf` command

## Shortcuts

| Key       | Action                          |
|-----------|---------------------------------|
| `Alt+S`   | Shelve current editor text      |
| `Alt+1-9` | Restore shelved prompt by number|
| `Alt+X`   | Clear all shelved prompts       |

## Command

| Command  | Description                          |
|----------|--------------------------------------|
| `/shelf` | Open shelf picker (restore / delete) |

## Installation

Copy `prompt-shelf.ts` to your Pi extensions directory:

```bash
cp prompt-shelf.ts ~/.pi/agent/extensions/prompt-shelf.ts
```

Pi will automatically load it on the next session.

## License

MIT
