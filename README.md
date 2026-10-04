# ELI5: explain anything to anyone

A [Claude Code](https://claude.com/claude-code) skill that explains a topic, piece of code, error or document at the level of whoever is listening: a five-year-old, a high-school student, your manager, an engineer, your parents. It changes vocabulary, comparisons, tone, depth and framing to fit.

## What it does

- **Works out the audience** from your request (default: a curious five-year-old)
- **Understands the source first**: reads the code, finds the root cause of the error, pulls out the key points
- **Builds the explanation** as: the point → one comparison from the listener's world → as much detail as they can use → why it matters to them
- **Stays honest**: it leaves detail out but doesn't add errors, and says where a comparison breaks down
- **Handles several audiences at once**: "explain this to my manager and to the engineers" gives two labelled versions

## Supported audiences

| Group | Examples |
|---|---|
| Age | 5, 10, 15, 20s–30s, 40+ |
| Schooling | Primary, middle school, high school, university, graduate/expert |
| Role | Manager, director, product manager, engineer, designer, colleague, client |
| Relationship | Partner, parents/grandparents, kids, friend |

Anyone else gets the same three questions: what do they already know, what do they care about, and how much time will they give you?

## Example prompts

```
ELI5 what a database index is
Explain this stack trace to my manager
Break down how git rebase works for a high-school student
How do I explain what a VPN is to my mum?
Explain this PR to our designer and to the backend team
```

## Install

Personal (all projects):

```bash
git clone https://github.com/galvadino/eli5.git
cp -r eli5/skills/eli5 ~/.claude/skills/eli5
```

Project only: copy `skills/eli5` into `.claude/skills/eli5` in your repo.

Then just ask Claude Code to "ELI5 this" or "explain this to my manager".

## Evals

`evals/evals.json` contains test prompts with what a good answer should do. Run each prompt with the skill installed and check the output against its expectations.

## Credits

Inspired by [DreambigOu/ELI5](https://github.com/dreambigou/eli5) (MIT). This is an independent rewrite.

## License

MIT
