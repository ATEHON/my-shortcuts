# For your AI: how to use My Shortcuts

This file tells you, the AI, how to apply the My Shortcuts skill well.
The skill itself is in `SKILL.md`.

## Your app has no skills feature?

That is fine. The skill is just text.

1. Open `SKILL.md` and copy everything from the line "# My Shortcuts" down to the line "END OF MY SHORTCUTS".
2. Paste it into your project instructions, or as the first message of a chat.
3. Then type "setup".

This works in ChatGPT, Claude, Gemini and most other chat apps.

## Start questions

These are also in `SKILL.md` under "First run". Ask them when the Voice Card still says "not set", or when the user types "setup". Ask all five in one short message. If the user skips one, use the default in brackets.

1. Which 3 tasks do you ask AI to do every week? (default: keep recap, reply and post)
2. Paste two short texts you wrote yourself, not with AI. A message, an email or a post, a few lines each. Pick texts without private details about other people (health, money, addresses). (default: no Voice Card yet, writing shortcuts use short, plain sentences)
3. Who reads your texts: clients, your team or followers? (default: clients)
4. Any words or phrases you never want to see? (default: none)
5. Which app are you using: ChatGPT, Claude or Gemini? (default: show the saving steps for all three)

## When to load it

- A message starts with a word from the Shelf, like "recap:", "reply:" or "post:".
- The user types "shortcuts", "add shortcut", "voice card" or "setup".
- The user asks to make a prompt they repeat into one word.

## When not to load it

- Normal questions that do not start with a trigger word.
- One-off tasks the user will not repeat.
- The user wants a full style analysis or wants a text checked for AI patterns. That is a different task.

## Typical mistakes

- **Describing instead of showing.** "Friendly but professional" sounds like everyone. Build the Voice Card from the user's own two texts. SAMPLE beats every other line.
- **Too many shortcuts.** More than 8 and the user forgets them. Ask which one to drop.
- **Voice Card on the wrong task.** Recaps, numbers, tables and summaries stay plain. Only "voice: yes" shortcuts use the Voice Card.
- **Forced phrases.** Putting every I SAY phrase into every text sounds like a parody. Use them where they fit.
- **Copying the sample.** Copy how the user writes, never what the sample says.
- **Warm up and sign off lines.** "Sure, here is your reply" and "Let me know if you need more" are not part of the output.
- **Invented facts.** If the input does not say it, write [check: ...] instead.
- **Half a file.** After a change, give the whole new file, not only the changed line. Unchanged parts stay word for word.

## What a good result looks like

Running a shortcut: only the result, in the format from the Shelf line.

After a change: the complete new file in one block fenced with four backticks, from `---` to `END OF MY SHORTCUTS`, then one line on how to save it in the user's app.

See `examples/` for a full before and after.
