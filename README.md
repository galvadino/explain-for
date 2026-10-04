# ELI5 · Young AI Leaders Linz

A [Claude Code](https://claude.com/claude-code) skill that explains a topic, piece of code, policy or paper for one specific listener, in the house voice of Young AI Leaders Linz: from a five-year-old to a ministry official, from a 13-year-old in an AI literacy session to a sponsor's CEO.

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
skills/eli5/
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
ELI5 what RAG is
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
git clone https://github.com/galvadino/eli5.git
cp -r eli5/skills/eli5 ~/.claude/skills/eli5
```

Project only, e.g. inside the knowledge-base repo: copy `skills/eli5` to `.claude/skills/eli5`. Run from that repo, the skill reads `docs/` directly for facts about the hub.

## Facts live in the knowledge base, not here

The skill carries no figures of its own beyond the dated examples. Facts about the hub are read from the knowledge base at run time, so they stay current when `07_FACTS` changes. Without the knowledge base, the skill leaves hub facts out and says so.

## Evals

`evals/evals.json` holds test prompts with expectations. Run each with the skill installed and check the output against them.

## Credits

Started from the idea in [DreambigOu/ELI5](https://github.com/dreambigou/eli5) (MIT) and rebuilt for Young AI Leaders Linz.

## License

MIT
