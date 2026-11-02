# My Shortcuts

**You type the same prompts every week, and the answers still do not sound like you. My Shortcuts puts your routines on one word each, plus a Voice Card built from your own texts.**

Works with Claude and Gemini as a skill, and with ChatGPT or any other chat app by copy and paste.

## What you get

One file with two parts:

| Part | What it is |
|---|---|
| The Shelf | Up to 8 of your own shortcuts. One word starts each one, like `recap:`, `reply:` or `post:` |
| The Voice Card | 5 lines about how you write: LENGTH, TONE, I SAY, I NEVER SAY, SAMPLE |

Each shortcut says what you paste in, what you get back, and if it should sound like you (`voice: yes`) or stay plain (`voice: no`).
Type `shortcuts` to see them all. Type `add shortcut` to make a new one.

Your AI cannot change the file by itself. After every change it gives you the full new file to save.

## Install and use in 3 steps

1. **Get the file.** Download `my-shortcuts.zip` from Releases.
2. **Add it to your AI.**
   - Claude: Customize, Skills, upload `my-shortcuts.zip` as it is (code execution must be on).
   - Gemini: Customize, Skills, upload `SKILL.md` from the ZIP (web or Mac app only, personal accounts 18+).
   - ChatGPT or any other app: open `SKILL.md`, copy everything from the line "# My Shortcuts" down to the line "END OF MY SHORTCUTS", and paste it into your project instructions or as the first message.
3. **Type "setup".** Answer five short questions. Save the new file your AI gives you. From then on, type `recap:` and paste your notes.

## Example

A made-up physio practice asks AI for the same three things every week.

| | Before | After |
|---|---|---|
| Instructions typed for 3 tasks | 555 characters | 17 characters (`recap:`, `reply:`, `post:`) |
| Reply to a patient | 78 words, "don't hesitate", formal sign off | 36 words, her own opening and sign off |

Reply after:

```
Hi Tom, quick one. Keep Thursday at 4. It's the last check before you run again. Until then a short, easy jog is fine. If it hurts, stop and tell me Thursday. See you then, Mara
```

Full example: `examples/before_typed_prompts.md` and `examples/after_my_shortcuts.md`.

## Files

| File | For whom |
|---|---|
| `SKILL.md` | Your AI. The skill itself, with your Shelf and Voice Card |
| `FOR_YOUR_AI.md` | Your AI. When to use it, start questions, common mistakes |
| `examples/` | You and your AI. One full before and after |
| `release/my-shortcuts.zip` | Ready to upload. Same files in a folder named `my-shortcuts` |
| `LICENSE` | MIT |

## License

MIT. Free to use, change and share.
