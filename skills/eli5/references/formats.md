# Formats

How an explanation is laid out, by where it will be used. Default to **Chat**. Switch only when the user names a use or a channel.

All layouts follow the house style: sentence-case headings, no emoji, no exclamation marks, figures with their scope, `·` for tight labels.

---

## Chat (default)

```
**<Takeaway, one sentence, in bold>**

<Bridge: one comparison from the listener's world, 1–3 sentences.>

<Detail: as many short paragraphs as this listener can use.>

**For you:** <what it means for this listener, one or two sentences.>

<Optional: "Where the comparison breaks: …" one line.>
<Optional: one follow-up offer, or for pupils one check question.>
```

For a five-year-old, drop the labels and keep it to a few sentences of plain prose.

## Multi-audience

One explanation per listener, each self-contained, in the order of the audience ladder (institutional first, family last).

```
### For · <Listener>
**<Takeaway>**
<Bridge, detail, for-you, scaled to this listener.>

### For · <Listener 2>
…
```

Then, if useful, one closing line on what stays true across all versions: the shared one-sentence core.

## Slide

One idea per slide. If it needs a paragraph, it is two slides or speaker notes.

```
Slide title (sentence case, a statement): <the takeaway, ≤ 10 words>
On the slide: <one comparison or one figure with its scope; ≤ 3 short lines>
Speaker notes: <the detail and the for-you, as you would say it aloud>
```

Figures and their scope go on the same slide at the same weight. Named institutions do the work, not adjectives. No build animations.

## School handout (AI literacy)

German by default for Austrian schools (*du* for pupils), A4, one page. Flag native-speaker review under the output.

```
# <Was ist …? / What is …?>  (the only H1)

**In einem Satz:** <takeaway>

## So kannst du es dir vorstellen
<one comparison from school or everyday life>

## Wie es funktioniert
<3–5 short steps or sentences>

## Darauf solltest du achten
<what it can get wrong; how to check it>

## Probier es aus
<one small task or question to check understanding>
```

Capability, not enthusiasm: the section on what to watch out for is never optional.

## LinkedIn post

Composed, specific, written for institutional readers and partners first.

```
<Line 1: the specific thing — a named body, a number, a shipped build — not a hook question.>

<2–4 short paragraphs: the comparison, the mechanism in plain words, why it matters.>

<One closing line: what it means for the reader, or what we are doing next.>
```

No emoji, no hashtag walls (at most two or three relevant tags at the end), no "I'm thrilled to announce", no rhetorical opener. Any figure about us comes from the knowledge base with its scope.

## One-page explainer (HTML)

When the user asks for a page, handout to share, or something visual, fill `assets/explainer.html`. It already carries the brand tokens and type. Rules it encodes:

- Paper background, ink text. Light only.
- Space Grotesk for headings, Inter for body, JetBrains Mono only for small data ticks (dates, a figure's label).
- The brand gradient only as a thin accent rule, never behind text and never behind a number.
- One H1. Body measure around 65–75 characters.
- Figures render in ink, with the scope label at the same size as the label.
- No icons of robots, brains or circuit boards; no stock imagery.

Replace every `{{…}}` placeholder; delete sections you do not use rather than leaving them empty.
