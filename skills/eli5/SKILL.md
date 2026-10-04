---
name: eli5
description: "Explain a topic, piece of code, error, document, or idea at the level of a specific audience. Use whenever the user says 'ELI5', 'explain like I'm …', 'explain this to my …', 'break this down for …', 'dumb it down', 'in plain English', 'simplify this for …', or 'how do I tell my boss/mom/team …'. Also use when the user names a listener (a kid, a grade level, a role like manager or designer, a family member, a friend) and wants something made understandable for them, or asks for one explanation at several levels. Partial phrasings like 'tell my boss' or 'explain to my dad' count."
---

# ELI5: explain anything to anyone

Your job is to get one idea from the source material into one specific person's head, using what that person already knows. The listener decides the words, the comparisons and the length, not the topic.

## 1. Figure out who is listening

Read the request for the audience. If none is named, use the classic ELI5 default: a curious five-year-old. If the user names more than one audience ("explain this to my manager and to the engineers"), write a separate, labelled explanation for each.

Place the listener in one of these groups and use the matching settings.

### By age

| Listener | Words | Comparisons drawn from | Feel |
|---|---|---|---|
| ~5 | Short, everyday words, short sentences | Toys, snacks, pets, the playground, bedtime | Delighted, a bit of wonder |
| ~10 | Simple, a few new words explained | School, sports, video games, building with blocks | Curious, cause and effect |
| ~15 | Normal teen vocabulary, some abstraction | Phones, group chats, games, streaming | Relaxed, never "hello fellow kids" |
| 20s–30s | Plain adult language | Rent, commuting, shopping, jobs | Direct |
| 40+ | Plain adult language, respectful | Running a household, a career, managing people | Unhurried, no condescension |

### By schooling

| Listener | How to pitch it |
|---|---|
| Primary / 5th grade | No jargon at all, concrete examples, "it's like…" |
| Middle school | Introduce one or two real terms, define each, walk step by step |
| High school | Use proper terms with a short gloss, allow moderate complexity |
| University | Technical terms with brief context; link theory to a practical case |
| Graduate / expert | Assume the basics; spend the words on nuance, trade-offs, edge cases, limits |

### By role

| Listener | What they want out of it | Lead with |
|---|---|---|
| Manager | Impact, risk, time, cost | What changes for the team and what decision is needed |
| Director / executive | Strategy, return, positioning | The one-line takeaway and why it matters for the business |
| Product manager | User value, scope, priority | Which user problem it touches and what to build or skip |
| Engineer | Mechanism, design, trade-offs | How it works and what is unusual about it |
| Designer | Experience, flow, accessibility | What the user sees, feels and can or cannot do |
| Colleague in another team | What it means for their work | What they need to know to work with you |
| Client / customer | Reassurance, outcome | What it means for them, in their words |

### By relationship

| Listener | Tone | Comparisons drawn from |
|---|---|---|
| Partner | Warm, conversational | Shared routines, the home, things you do together |
| Parents / grandparents | Patient, respectful | Technology they already use, post, bank, kitchen, phone calls |
| Your kids | Playful, short | Cartoons, games, school, animals |
| Friend | Casual, a little humour | Pop culture, shared hobbies, "you know when…" |

If the listener fits none of these, ask yourself three things and act on the answers: what do they already know, what do they care about, and how much time will they give you.

## 2. Understand it yourself first

You cannot simplify what you have not understood. Before writing:

- **Code**: read the actual files. Work out what the code is *for* before how it does it.
- **An error**: find the root cause, not just the message text.
- **A concept**: break it into its two or three essential parts.
- **A document**: pull out the points that matter to this listener.

Then write down, for yourself, the single sentence you want the listener to remember. Everything else serves that sentence.

## 3. Build the explanation

Use this shape, stretched or shrunk to fit the listener:

1. **The point**: one sentence saying what it is.
2. **The bridge**: one comparison to something the listener already knows well. Pick a single comparison and stay with it rather than stacking several.
3. **The detail**: add only as many layers as this listener can use. For a five-year-old that may be zero; for an engineer it is most of the answer.
4. **Why it matters to them**: close on what this means for *this* person, such as a decision, a risk, a reason to care, or something they can now do.

### Calibrate the language

**Non-technical listeners** (kids, family, most business roles):
- No jargon. If a term is unavoidable, define it in the same sentence.
- One idea per sentence.
- Concrete beats abstract: "the server is the kitchen, your browser is the customer ordering" beats "the server processes client requests".
- Talk to them: "you", "your".

**Technical listeners** (engineers, grad students, experts):
- Use correct terminology; avoiding it reads as patronising.
- Skip what they know; compare to what they know ("like a hash map, except…").
- Spend the words on the interesting part: trade-offs, failure modes, why it was designed this way.

**Business listeners** (managers, directors, clients):
- Outcome first, mechanism later or never.
- Put numbers on things where you honestly can (time, cost, users affected).
- End with the decision or the ask.

### Keep it honest

- Simplifying is fine; saying something false is not. Leave detail out, but don't put errors in. If the comparison breaks down in a way that matters, say so in a line ("the difference is…").
- For a very non-technical listener, getting 80% of the idea across clearly beats 100% that loses them. Pick the 80% that stays true.

### Length

Match length to the listener: a few sentences for a young child, a short paragraph or two for most adults, as much as needed for an expert who asked for depth. Stop when the takeaway has landed.

## 4. Offer a next step (optional)

When it helps, close with one line that invites a follow-up at the right level, e.g. "Want the version with the actual numbers?" or a question a kid could answer to check they got it. Don't add this to every answer.

## Examples

**"ELI5 what a database index is"** (no audience, so default to five years old)

> You know how a big picture book about animals has a page at the front that says "Lions: page 12, Penguins: page 40"? Without it, you'd have to flip through every page to find the penguins. A database index is that page at the front. It tells the computer exactly where to look, so it finds things super fast.

**"Explain our API rate limit problem to my manager"**

> Our payment provider only lets us send 100 requests a minute. At lunchtime we go over that, so about 3% of checkouts fail and customers have to retry. Two ways out: two days of engineering work to batch our calls, or move to their higher plan for roughly €200 a month. I'd do the engineering fix; it also makes us faster. I need a yes on which one by Friday.

**"Explain React's useEffect to a university student"**

> `useEffect` is where a React component does work that isn't just drawing the UI, such as fetching data, subscribing to something, or touching the DOM directly. React runs it after rendering. The dependency array tells React when to run it again: empty means once after the first render, `[userId]` means whenever `userId` changes. If you return a function, React calls it as cleanup before the next run or when the component disappears. If you've seen class components, it folds `componentDidMount`, `componentDidUpdate` and `componentWillUnmount` into one place.

**"Explain what a VPN is to my mum and to our security engineer"** (two audiences, two labelled answers)

> **For Mum:** When you use the internet in a café, it's a bit like sending postcards: anyone handling them could read them. A VPN puts each postcard in a locked envelope and sends it to a trusted post office first, which then forwards it. People in the café can see you're sending mail, but not what it says or where it's really going.
>
> **For the security engineer:** An encrypted tunnel (typically WireGuard or IPsec) from the client to a VPN gateway; the gateway egresses traffic, so the local network sees only tunnel traffic to one endpoint. It shifts trust from the local network to the VPN operator rather than removing it, and doesn't help against endpoint compromise or DNS leaks if split tunnelling is misconfigured.

## Ground rules

- Never talk down. A five-year-old's version should feel like a treat, and a manager's version should leave them better equipped to decide.
- With code, explain the purpose before the mechanism. Nobody cares about syntax until they know why it exists.
- Use the listener's world for comparisons, not yours.
- One clear idea that sticks is better than five that blur.
