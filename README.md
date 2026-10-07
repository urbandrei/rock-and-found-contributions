# Translate Rock and Found

[Rock and Found](https://store.steampowered.com/app/5203560/Rock_and_Found/) is a cozy game about
identifying rocks and putting them back where they belong, in the museum a grandmother built and
never opened. Its demo is free on Steam and itch.io.

This is where players help translate it. Everything here is the English text of the demo, ready
for translation into any language.

## How it works

- **It is voluntary and unpaid.** You choose what to translate and when. There are no deadlines,
  and you can stop at any time.
- **You are credited** in the game under "Community translation", with the name you choose, or
  anonymously if you prefer.
- **Thank you keys.** Active translators get a free Steam key for the full game when it comes out.
- **Human translation only.** No machine translation, no AI tools, no "pre-translate" buttons. The
  game is made by hand, and the translations should be too.
- **Paid translations may come later.** If the game does well, professional translators may build
  on your work, edit it or replace it. You stay credited either way.
- **You must be 18 or older.**

## Before you start: the agreement

Please read [AGREEMENT.txt](AGREEMENT.txt). It explains, in plain words, what you allow when you
contribute. Then send this sentence, with your credit name filled in, to the Rock and Found Discord
or to support@rockandfound.com:

> I have read the Rock and Found Contributor Agreement, Version 1 (October 7, 2026). I agree to
> it, and I am 18 or older. Please credit me as: ________.

The agreement's fingerprint (SHA-256), so anyone can check it is the same text:

```
bddfdd1c3fc637a35dde39138a9e31d54e13034b996ed5546a8db63a5633ab9a
```

## Languages

One lead per language keeps everyone from translating the same lines twice. If your language has
a lead, ask them how to help. If it is open, say hello and it can be yours.

| Language | Lead | Status |
|---|---|---|
| French (Français) | (open) | open |
| German (Deutsch) | (open) | open |
| Spanish (Español) | (open) | open |
| Portuguese, Brazil (Português) | (open) | open |
| Italian (Italiano) | (open) | open |
| Polish (Polski) | (open) | open |
| Russian (Русский) | (open) | open |
| Ukrainian (Українська) | (open) | open |
| Chinese, Simplified (简体中文) | (open) | open |
| Japanese (日本語) | (open) | open |
| Korean (한국어) | (open) | open |

Your language is not listed? Ask. Any language is welcome.

## What to translate

- `rockandfound.pot` is every line of English in the demo: the menus, the tutorial notes, the
  journal, the stone names, the room plans and the first four letters. About 5,700 words.
- `suggestions/` has a starting file for several languages, with some lines already filled in
  (see below). If your language is there, start from that file.

Each line has a **context** and often a **note**:

| Context | What it is |
|---|---|
| `kind` | The name of a stone, mineral or fossil. Use the usual name in your language. Keep it short: it goes on small brass tags. |
| `journal` | Grandma's journal notes about a stone. Short and plain on purpose: they sit on small pages. |
| `letter` | Rose's handwritten letters. These matter most for the story. Take your time. |
| `letter paper` | Words printed on the paper a letter came on (a postcard, an order form). Optional: leave it empty to keep the American original. |
| `map` | Room names and the places on the room plans. |
| (others, or none) | Menus, notes, prompts, settings and everything else. |

## Suggestions: stone names and dates, already looked up

So you can spend your time on the journal and the letters, the files in `suggestions/` come with
some lines filled in:

- **Stone, mineral and fossil names** that are real minerals or rocks, taken from
  [Wikidata](https://www.wikidata.org) and checked against the matching Wikipedia article title.
- **Month names and the date order**, from the Unicode CLDR (the data your phone and computer use
  for dates).

These come from reference data entered by people, not machine translation. **Every one is marked
"needs work" and is not used by the game until you confirm it.** Check each one, fix it if needed,
and turn "needs work" off. The comment above each line says where it came from. Names the game made
up ("Purple Cubes") and every menu word are left for you.

## Rules

- **Keep the placeholders exactly:** `%d`, `%s`, and names in braces like `{done}`. You can move
  them within the sentence, but do not change, translate or remove them.
- **Keep blank lines** inside a letter: each blank line starts a new paragraph.
- **Keep it about as long as the English.** Longer text is made smaller to fit, and very long text
  gets hard to read.
- **Rose and Delilah.** Do not add family words (mother, grandmother, daughter, aunt) that the
  English line does not use. Some of the story depends on it. If a line is unclear, ask.
- **Mineral names:** the standard name in your language, the one a rock shop or museum would use.
  If there is none, keep the English name. Keep chemical formulas (SiO2, CaCO3) as they are.
- **Hardness** is the Mohs scale; **streak** is the color of a stone's powder on a porcelain plate.
- **Tone:** warm, quiet, plain. Short sentences. Nothing jokey that the English does not have.

## How to translate

1. Install [Poedit](https://poedit.net) (free).
2. Open your language's file in `suggestions/` and save it under your own name. If there is none,
   choose **File, New from POT/PO file**, open `rockandfound.pot` and pick your language.
3. Translate. Save often.
4. Send the `.po` file to your language's lead, or to the Discord or support@rockandfound.com.

When the English changes, a new `rockandfound.pot` appears here. In Poedit use **Translation,
Update from POT file**: changed lines are marked "needs work" and new lines show up empty.

## See your translation in the game

From demo version 0.0.4 on, you can test your file in the demo itself:

1. On Windows, press Win+R and paste `%APPDATA%\Godot\app_userdata\Rock and Found`
2. Make a folder there called `locale` and put your `.po` file in it.
3. Start the demo. Your language shows on the journal's settings page, marked "(testing)".

Your file stays on your computer. Look for text that runs off a page, letters that show as empty
boxes, and lines that read oddly in context, and send a screenshot of anything that looks wrong.

## The small print

The English text is by Andrei Roman, and you may translate it for Rock and Found. Please do not
reuse it for anything else. [NOTICE.txt](NOTICE.txt) lists the sources of the suggestions and their
licenses.
