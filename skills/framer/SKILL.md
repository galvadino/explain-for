---
name: framer
description: "Frame a topic, document, piece of code, error, policy, paper, agenda or idea for one specific listener. Use whenever the user says 'frame this for …', 'explain this to …', 'break this down for …', 'in plain English', 'simplify this for …', 'what does this mean for …', 'how do I tell …', or names a listener and wants something made understandable: a child or teenager, a student, a manager, executive or board, an engineer, designer or researcher, a public official or funder, a customer, a journalist, a team, or family and friends. Also use for one idea framed for several listeners at once, for turning an explanation into a slide, handout, email, social post or one-page explainer, and for explanations in another language. Partial phrasings like 'tell my boss' or 'explain to the class' count."
---

# Framer

**Same facts. The right frame.**

A frame is every choice that decides whether an idea lands: what comes first, which comparison carries it, how deep it goes, what it means for the person listening, and the language and layout it arrives in. Framer makes those choices for one listener at a time.

Two things stay fixed, whoever is listening: the source decides what is true, and the voice stays clear and exact. The listener decides everything else.

Four reference files sit next to this one. Read them when the step calls for them:

- `references/listeners.md`: listener profiles, with what each needs, what loses them and what to lead with
- `references/voice.md`: the default voice, banned hype, punctuation, numbers, dates, languages
- `references/formats.md`: layouts (chat, several listeners, slide, handout, email, social post, one-page HTML)
- `references/examples.md`: worked examples, from a five-year-old to a minister, in English and German

## 1. Identify the listener

Read the request for who is listening and where it will be used.

- **Named listener**: look them up in `references/listeners.md`.
- **No listener named**: a curious non-specialist adult, in plain language. If the use clearly matters (a deck, a handout, a letter) and the listener is unclear, ask one short question first.
- **Several listeners**: a separate, labelled frame for each, in the multi-listener layout.
- **Listener not in the file**: answer three questions and act on them: what do they already know, what do they care about, how much time will they give you.

Also settle the **language**: the listener's, which may differ from the user's. Pick the right form of address (*Sie* or *du*, *vous* or *tu*) for the relationship. Anything in a language other than the user's that is meant for publication or print is a draft until a native speaker reviews it; say so in one line under the output.

## 2. Understand it yourself first

You cannot frame what you have not understood.

- **Code**: read the files. Work out what it is *for* before how it works.
- **An error**: find the root cause, not just the message.
- **A document, agenda, policy or paper**: pull out what it is, what changes, for whom, when, and what the listener could do with it.
- **A concept**: reduce it to its two or three essential parts.

Then write, for yourself only, the **one sentence** the listener should remember. Everything else serves that sentence.

## 3. Keep the facts fixed

The frame changes; the facts do not.

- Take names, numbers, dates and titles **from the source**, exactly as written. Do not add figures, dates or details the source does not contain, and do not fill gaps from memory when the stakes are real. If something the listener will want is missing, say it is missing.
- **Keep the scope with every figure**, in the same sentence: whose number, over what period, for which group. "500 applications" and "500 applications across 13 cities" are different claims.
- Do not upgrade a relationship or status: a speaker is not a partner, a draft is not a decision, "proposed" is not "agreed", "upcoming" is not "done".
- If two sources disagree, show both and say which one you followed and why.
- **Project rules win.** If the working directory has a style guide, brand guide, glossary, facts file or `CLAUDE.md` with rules about voice, names or claims, follow them over the defaults in this skill.

## 4. Build the frame

The shape, stretched or shrunk to fit:

1. **Takeaway**: one sentence saying what it is. Lead with the specific: a named thing, a number, a concrete action.
2. **Bridge**: one comparison from the listener's world. One, held all the way through, not three stacked.
3. **Detail**: only as many layers as this listener can use. Zero for a five-year-old, most of the answer for an engineer.
4. **For you**: what it means for *this* listener: a decision, a risk, something they can now do or judge.

Then calibrate:

- **Non-technical listeners**: no jargon; if a term is unavoidable, define it in the same sentence. One idea per sentence. Concrete over abstract.
- **Technical listeners**: correct terminology, skip the basics, spend the words on trade-offs, failure modes and design choices.
- **Decision-makers** (executives, officials, funders): outcome first, mechanism only if asked. Name bodies, dates and amounts instead of using adjectives. End with the decision or the ask.

### Leave them able to judge

When the topic is a technology, especially AI, aim for **capability, not enthusiasm**: the listener should be better able to judge it, not just more excited or more scared. Where it fits, add one line on what it gets wrong or how to check it.

### Keep it true

- Simplify by leaving detail out, never by putting errors in.
- If the comparison breaks in a way that matters, say where in one line ("Where the comparison breaks: …").
- For a very non-technical listener, a clear 80% beats a complete version that loses them. Choose the 80% that stays true.

## 5. Write it clear and exact

Energy comes from specific nouns, strong verbs and short sentences, not from decoration. Full defaults in `references/voice.md`. The ones broken most often:

- No hype: no *groundbreaking, cutting-edge, world-class, revolutionary, game-changer*; no *empowering, unlocking, harnessing, transforming*.
- No emoji and no exclamation marks, unless the listener's register clearly calls for them (a note to a child, a casual message to a friend) or the project's style guide allows them.
- Say what something is, not what it is not ("not just a chatbot").
- Sentence case for headings. Unambiguous dates: `7 Oct 2026`, ranges `7–8 Oct 2026`.

Temperature changes by listener; clarity does not. Formal listeners get flatter, more formal sentences. Family and children get warmth, from patience and a good comparison rather than from punctuation.

## 6. Pick the layout

Default to a chat answer. Switch layouts when the user names a use: "for a slide", "as a handout", "as an email", "for LinkedIn", "make it a page". Layouts are in `references/formats.md`; the one-page template is `assets/explainer.html`.

Length follows the listener: a few sentences for a child, one or two short paragraphs for most adults, as much as needed for an expert who asked for depth. Stop when the takeaway has landed.

Close, when it helps, with **one** follow-up offer at the right level ("Want the version with the numbers?") or, for a learner, one question they can answer to check they got it. Not on every answer.

## Before you hand it over

Run these silently and fix anything that fails. Mention them only if something was left out or needs review.

1. **Listener**: would this person understand every sentence, and would they feel respected?
2. **Truth**: is anything false, or did a comparison sneak in an error?
3. **Facts**: does every name, number and date come from the source, with its scope, and is its status still accurate?
4. **Voice**: no hype, no negation framing, emoji and exclamation marks only where the register calls for them.
5. **Room test**: would you be comfortable if the most senior person who might see this read it?
