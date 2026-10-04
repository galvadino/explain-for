# Framer

**Same facts. The right frame.**

A [Claude Code](https://claude.com/claude-code) skill that frames one idea for one listener: a five-year-old, a class of 13-year-olds, your manager, an engineer, a minister, your mum.

A frame is every choice that decides whether an idea lands: what comes first, which comparison carries it, how deep it goes, what it means for the listener, and the language and layout it arrives in. Framer makes those choices per listener. The facts stay fixed, so the minister and the five-year-old hear different words but the same truth.

```
/framer this conference agenda for my manager
```

## What it does

- **Finds the listener**: decision-makers, colleagues, learners, the public and press, ages, school levels, family. For anyone else, it asks what they know, what they care about and how much time they will give you
- **Understands the source first**: reads the code, finds the root cause, pulls out what a document changes, for whom and when
- **Keeps the facts fixed**: names, numbers and dates come from the source exactly, with their scope; it never upgrades a status or fills gaps from memory, and it says when something is missing
- **Builds the frame**: takeaway → one comparison from the listener's world → detail they can use → what it means for them
- **Writes clear and exact**: specific nouns, strong verbs, no hype words, no "not just a …" framing
- **Leaves people able to judge**: on technology topics, one line on what it gets wrong or how to check it
- **Works in any language**, with the right form of address, and flags translations for native review
- **Lays it out** for the use: chat answer, several listeners at once, slide with speaker notes, handout, email, social post, or a one-page HTML explainer
- **Follows your project's rules**: if the repo has a style guide, brand guide, glossary or `CLAUDE.md`, those win over the defaults

## Structure

```
skills/framer/
├── SKILL.md                  the workflow
├── references/
│   ├── listeners.md          listener profiles
│   ├── voice.md              default voice, numbers, dates, languages
│   ├── formats.md            layouts
│   └── examples.md           worked examples, EN and DE
└── assets/
    └── explainer.html        one-page template with swappable design tokens
evals/
└── evals.json                test prompts with expectations
```

## Example prompts

```
Explain what RAG is to a five-year-old
Frame the EU AI Act risk levels for our CEO
Explain AI hallucinations to 13-year-olds, as a German handout
Explain what a VPN is to my mum and to our security engineer
Here's the conference agenda. Tell my manager why I should go.
Turn this explanation of embeddings into one slide
Write an email explaining this outage to our customers
```

## Install

Personal (all projects):

```bash
git clone https://github.com/galvadino/framer.git
cp -r framer/skills/framer ~/.claude/skills/framer
```

Project only: copy `skills/framer` to `.claude/skills/framer` in your repo.

## Make it yours

The defaults are deliberately plain. To fit your organisation, add a style guide, brand guide or facts file to your project (or a few lines in `CLAUDE.md`): Framer follows those over its own defaults. To restyle the one-page explainer, swap the design tokens at the top of `assets/explainer.html`.

## Evals

`evals/evals.json` holds test prompts with expectations. Run each with the skill installed and check the output against them.

## License

MIT
