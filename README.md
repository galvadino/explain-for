# Framer

**Same facts. The right frame.**

A [Claude Code](https://claude.com/claude-code) skill from Young AI Leaders Linz that frames one idea for one listener: a 13-year-old in an AI literacy session, a sponsor's CEO, a ministry official, the dinner table.

The frame is every choice that decides whether an idea lands: what comes first, which comparison carries it, how deep it goes, what it means for the listener, and the language and layout it arrives in. Framer makes those choices per listener. The facts come from the knowledge base and the voice from the house style, so both hold steady in every room.

```
/framer the EU AI Act risk levels for our sponsor's CEO
```

## What it does

- **Finds the listener** in a profile set built around how the hub works: institutional readers, partners and sponsors, prospective and new members, pupils, teachers and parents, panel audiences and press, engineers and other hub leads, ages, school levels, family
- **Understands the source first**: reads the code, finds the root cause, pulls out what a regulation changes and for whom
- **Checks any fact about the hub** against the knowledge base (`docs/CONTEXT.md`, `docs/LAWS.md`, `docs/07_FACTS/`): exact phrasing, scope with every figure, labels as ruled, nothing unverified, and omits what it cannot source
- **Builds the explanation** as takeaway → one comparison from the listener's world → detail they can use → what it means for them
- **Writes in the house voice**: high-energy, low-hype; no emoji, no exclamation marks, no superlatives or buzzwords, no negation framing; house punctuation, dates and names
- **Applies AI literacy rules** for pupils and the public: capability, not enthusiasm, with one line on what AI gets wrong or how to check it
- **Switches to German** for Austrian schools and public bodies (*du* / *Sie*), and flags drafts for native-speaker review
- **Lays it out** for the use: chat answer, multi-audience brief, slide with speaker notes, school handout, LinkedIn post, or a one-page HTML explainer in the brand palette and type

## Structure

```
skills/framer/
├── SKILL.md                  the workflow
├── references/
│   ├── audiences.md          listener profiles
│   ├── house-style.md        voice, punctuation, numbers, names, language
│   ├── formats.md            output layouts
│   └── examples.md           worked examples, EN and DE
└── assets/
    └── explainer.html        branded one-page template
evals/
└── evals.json                test prompts with expectations
```

## Example prompts

```
Frame what RAG is for a five-year-old
Explain the EU AI Act risk levels to our sponsor's CEO
Explain AI hallucinations to 13-year-olds, as a handout
Explain our Gambia project to a ministry official and to a prospective member
Turn this explanation of embeddings into one slide
Explain what an MCP server is to the Community & Events team
How do I explain to my parents what Young AI Leaders Linz is?
```

## Install

Personal (all projects):

```bash
git clone https://github.com/galvadino/framer.git
cp -r framer/skills/framer ~/.claude/skills/framer
```

Project only, e.g. inside the knowledge-base repo: copy `skills/framer` to `.claude/skills/framer`. Run from that repo, the skill reads `docs/` directly for facts about the hub.

## Facts live in the knowledge base, not here

The skill carries no figures of its own beyond the dated examples. Facts about the hub are read from the knowledge base at run time, so they stay current when `07_FACTS` changes. Without the knowledge base, the skill leaves hub facts out and says so.

## Evals

`evals/evals.json` holds test prompts with expectations. Run each with the skill installed and check the output against them.

## License

MIT
