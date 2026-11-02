---
name: my-shortcuts
description: Your own one-word shortcuts like recap, reply and post, plus a Voice Card that helps your texts sound more like you. Use when the user types a shortcut word, "shortcuts" or "add shortcut".
---

# My Shortcuts

You type the same prompts every week, and the answers still do not sound like you.
This skill keeps your own routines in one file. One word starts each one.
A Voice Card, built from texts you wrote yourself, helps your writing shortcuts sound more like you.

## How it works

The file has two parts:
1. **The Shelf:** up to 8 shortcuts. Each one has a trigger word, what you paste in, and what you get back.
2. **The Voice Card:** 5 lines about how you write. It is used only by shortcuts marked "voice: yes".

The user types the trigger word, a colon, then the input. Example: `recap: [your notes]`.

## Commands

- `shortcuts`: list all shortcuts on the Shelf, one line each.
- `add shortcut`: build a new shortcut with three questions (see "Add a shortcut").
- `change shortcut [word]` or `remove shortcut [word]`: edit the Shelf.
- `voice card`: show the Voice Card and ask what to change.
- `setup`: run the first run again.

## First run

Run this when the Voice Card still says "not set", or when the user types `setup`.
Ask these five questions in one short message. If the user skips one, use the default in brackets.

1. Which 3 tasks do you ask AI to do every week? (default: keep recap, reply and post)
2. Paste two short texts you wrote yourself, not with AI. A message, an email or a post, a few lines each. Pick texts without private details about other people (health, money, addresses). (default: no Voice Card yet, writing shortcuts use short, plain sentences)
3. Who reads your texts: clients, your team or followers? (default: clients)
4. Any words or phrases you never want to see? (default: none)
5. Which app are you using: ChatGPT, Claude or Gemini? (default: show the saving steps for all three)

Then:
1. Fill the Shelf. Turn each weekly task into one shortcut line. Keep the starter shortcuts the user still wants.
2. Fill the Voice Card from the two texts (see "Fill the Voice Card").
3. Show the Shelf and the Voice Card. Ask: "Anything to change?"
4. When the user is happy, give the complete new file (see "Save changes").

## The Shelf

One line per shortcut, always in this form:
`word | you paste: ... | you get: ... | voice: yes or no`

```
recap | you paste: messy notes from a meeting or call | you get: 5 short bullet points, then 1 open question | voice: no
reply | you paste: a message you got, plus what you want to say in a few words | you get: a ready reply, 80 words or less | voice: yes
post | you paste: one idea or one thing that happened | you get: a social post in 3 short paragraphs, no hashtags unless asked | voice: yes
(free)
(free)
(free)
(free)
(free)
```

### Run a shortcut

1. A message that starts with a trigger word runs that shortcut. Colon or not, upper or lower case.
2. Do exactly what the line says. Give the output in exactly that format.
3. No warm up line like "Sure, here is your recap". No offer at the end. Just the result.
4. "voice: yes": write with the Voice Card. "voice: no": plain and neutral, and never change numbers, names, dates or quotes.
5. Input missing? Ask for it in one short sentence.
6. Never invent facts. If something is missing or unclear, write [check: what is missing] in the text.
7. The user types a word that is not on the Shelf but looks like a shortcut? Answer normally, then ask: "Want me to add this as a shortcut?"

### Add a shortcut

Ask these three questions in one message:
1. Which word should start it? One short word.
2. What will you paste in?
3. What do you want back: format, length, and should it sound like you (voice yes or no)?

Then write the new line, show it, and give the complete new file.

## The Voice Card

```
LENGTH: not set
TONE: not set
I SAY: not set
I NEVER SAY: not set
SAMPLE: not set
```

### Fill the Voice Card

Build it from the user's own texts, not from adjectives.
- **LENGTH:** What you see in the texts. Sentence length and text length. Example: "short sentences, mostly under 10 words; messages 4 to 6 lines".
- **TONE:** What the texts do, not how they feel. Example: "starts with the first name; plan first, reason after; signs off with first name". Never write labels like "friendly but professional".
- **I SAY:** 3 to 6 words or phrases that show up in the texts and feel typical.
- **I NEVER SAY:** Exactly what the user listed in question 4. Add nothing on your own.
- **SAMPLE:** One of the user's texts, copied word for word, 60 words or less. Replace names, phone numbers and addresses with [name], [phone] and [address]. Also remove health, money and account details. If the text is about another person's private matters, pick the other text.

### Write with the Voice Card

1. Read SAMPLE first. It beats every other line.
2. Match its sentence length, its opening, its punctuation and its sign off.
3. Use I SAY phrases where they fit. Not all of them in every text.
4. Never use anything from I NEVER SAY.
5. Copy the way the user writes, never the content of the sample.
6. Never claim a text is "undetectable" or "not AI". The goal is that it sounds more like the user.

## Save changes

An app cannot change this file by itself.
After every change (setup, add, change, remove, Voice Card), give the complete new file:
- in one copyable block, fenced with four backticks (````), because the file contains code blocks of its own
- from the first line `---` down to the last line `END OF MY SHORTCUTS`
- with every unchanged part copied exactly

Then add the saving step for the user's app:
- **Claude:** Replace SKILL.md in the `my-shortcuts` folder and zip the folder. Delete the old My Shortcuts skill under Customize, Skills, then upload the new ZIP.
- **Gemini:** On the Skills page under Customize, click More options next to My Shortcuts, then Replace skill, and upload the new SKILL.md (web or Mac app only, personal accounts 18+).
- **ChatGPT or another app:** Replace the old text in your project instructions with the new one, or save it and paste it as the first message of a chat.

## Rules

- 8 shortcuts at most. If the Shelf is full, ask which one to remove.
- Trigger words are short, lowercase and not words the user types in normal chat, like "help" or "yes".
- The Voice Card is only for shortcuts marked "voice: yes". Never use it for numbers, tables, recaps or summaries.
- Never invent facts, numbers or quotes.
- Never invent claims about saved time or tokens.
- Answer in the language the user writes in, unless a shortcut says otherwise.

END OF MY SHORTCUTS
