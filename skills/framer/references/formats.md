# Formats

How a frame is laid out, by where it will be used. Default to **Chat**. Switch only when the user names a use or a channel.

All layouts: sentence-case headings, figures with their scope, `·` for tight labels, the voice defaults in `voice.md`.

---

## Chat (default)

```
**<Takeaway, one sentence, in bold>**

<Bridge: one comparison from the listener's world, 1–3 sentences.>

<Detail: as many short paragraphs as this listener can use.>

**For you:** <what it means for this listener, one or two sentences.>

<Optional: "Where the comparison breaks: …" one line.>
<Optional: one follow-up offer, or for a learner one check question.>
```

For a young child, drop the labels and keep it to a few sentences of plain prose.

## Several listeners

One frame per listener, each self-contained. Order them from most formal to least.

```
### For · <Listener>
**<Takeaway>**
<Bridge, detail, for-you, scaled to this listener.>

### For · <Listener 2>
…
```

If useful, close with one line naming the core that stays the same in every frame.

## Slide

One idea per slide. If it needs a paragraph, it is two slides or speaker notes.

```
Slide title (a statement, sentence case, ≤ 10 words): <the takeaway>
On the slide: <one comparison or one figure with its scope; ≤ 3 short lines>
Speaker notes: <the detail and the for-you, as you would say it aloud>
```

Keep a figure and its scope on the same slide at the same weight. No build animations.

## Handout

One page, for learners or a general audience. Only one H1.

```
# <What is …?>

**In one sentence:** <takeaway>

## Think of it like this
<one comparison>

## How it works
<3–5 short steps or sentences>

## What to watch out for
<what it gets wrong; how to check it>

## Try it
<one small task or question to check understanding>
```

For a technology topic the "What to watch out for" section is never optional. In another language, translate the headings and flag native-speaker review.

## Email

```
Subject: <the takeaway, ≤ 8 words, no clickbait>

<Line 1: the takeaway, or what you need from them.>
<1–2 short paragraphs: the comparison and the detail they need.>
<Last line: the decision, the ask or the next step, with a date if there is one.>
```

## Social post

```
<Line 1: the specific thing — a named body, a number, a concrete result — not a hook question.>

<2–4 short paragraphs: the comparison, the mechanism in plain words, why it matters.>

<One closing line: what it means for the reader, or what happens next.>
```

No hashtag walls (two or three relevant tags at most), no "thrilled to announce", no rhetorical opener.

## One-page explainer (HTML)

When the user asks for a page, a shareable handout or something visual, fill `assets/explainer.html`.

- The design tokens are grouped at the top of the file. Swap them for a project's brand if it has one; otherwise keep the neutral defaults.
- One H1. Body measure around 65–75 characters.
- Figures in the text colour, never on a coloured background, with the scope label at the same size as the label.
- The accent colour is for one thin rule and links only.
- No stock imagery and no AI clichés (glowing brains, robots, circuit boards).

Replace every `{{…}}` placeholder; delete sections you do not use rather than leaving them empty.
