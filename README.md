# Concept Check

**Test whether a concept earns its place in your argument.**

A Claude skill for researchers and writers in the humanities and social sciences. It takes a term you coined or lean on, sets it against the alternatives you could have used, and shows what the concept gains you and what it costs.

Built on John Gerring's criteria for good concepts and Giovanni Sartori's test for conceptual stretching.

<img width="750" alt="Concept Check" src="assets/concept-check.jpg" />

[Download `concept-check.zip`](https://github.com/Halfofthesky/concept-check/releases/latest/download/concept-check.zip) · [View `SKILL.md`](concept-check/SKILL.md)

---

## When you need it

- You've **coined a term**, and you need to know whether it beats the words that already exist.
- Your argument **rests on one big word** (populism, memory, care, resilience, ideology) and a reviewer could ask, "what exactly do you mean?"
- You're **applying a concept to new cases** and suspect it no longer fits them.
- You're **reading a theory-heavy text** and want to see what its central concept really does.
- You're **writing in two languages**, and the term that works in one may fail in the other.

## Why you need it

Concepts are where humanities and social-science writing takes its biggest risks and gets the least feedback. Reviewers say a term is "vague" or "unnecessary," but rarely say why, or what to do about it.

There is no perfect concept. Every choice trades something away:

- A familiar term may be too loose.
- A sharp definition may sound strange.
- A catchy coinage may poach from neighbouring terms.

Gerring's point is that these costs can be named, and judged against the alternatives you had. This skill does exactly that.

## What it does

It reads your text and produces:

1. **A concept card**: the term, every definition the text gives (quoted, with location), the defining attributes, the cases covered, and the definition strategy (minimal, ideal type or cumulative).
2. **A uses table**: every significant use of the term, so you can see whether its meaning drifts.
3. **A trade-off table**: the concept set against two or three real alternatives (the nearest existing term, a rival definition, a narrower or broader version of your own), criterion by criterion: *gain / cost / neutral / n.a.*, with evidence. No scores.
4. **Flags**, each with its location in the text:

| Flag | What it catches |
|---|---|
| F1 Stretching | The concept applied to cases its attributes don't fit |
| F2 Drift | The meaning shifts within the same work |
| F3 Unargued neologism | A new term with no reason why existing ones fail |
| F4 Missing contrast | The text never says what the concept is *not* |
| F5 Relabelling | A new name for an old bundle, or attributes taken from a neighbouring term |
| F6 Incoherent bundle | Defining attributes that don't belong together |
| F7 Shallow | A concept defined mostly by what it isn't |
| F8 Strategy mismatch | An ideal type used as a yes/no category, or the reverse |
| F9 Idle concept | Swap in an existing term and nothing in the argument changes |
| F10 Unrecognisable | No way to tell an instance from a non-instance |
| F11 Ambiguous | Two readings the text can't decide between, given both |

5. **Moves**: concrete options (rename, add or drop an attribute, narrow the scope, state the contrast, split the concept), each with what it improves and what it costs.

It **doesn't rewrite your text** or rate your concept on a scale. It never treats a criterion as a rule.

### The criteria

| Criterion | The question |
|---|---|
| Familiarity | Does it fit how the term is already used? |
| Click | Does it stick? |
| Parsimony | Is it short, with few defining attributes? |
| Domain | Which readers and which cases is it meant for? |
| Consistency | Does it mean the same thing throughout? |
| Coherence and depth | Do its attributes belong together, and do its cases share more than the definition? |
| Differentiation | Where does it end and its neighbours begin? |
| Field utility | Does it leave neighbouring terms intact? |
| Theoretical utility | What would the argument lose without it? |
| Recognition | Can a reader tell an instance when they see one? |

## How to use it

Give Claude your text (or a section of it) and say what you want. Three modes:

- **Audit**: your own draft. *"Run a concept check on 'telescoping' in this chapter."*
- **Read**: someone else's text. *"Concept-check 'governmentality' in this article: what does it buy the argument?"*
- **Design**: a concept you're still forming. *"I want a term for X. Here are my notes. Help me design the concept."*

If you don't name a concept, it picks the terms the argument depends on and tells you which. It checks one to three concepts per run, and works in any language.

**Tip:** name the alternatives you care about ("compare it with 'acceleration'"). The comparison is where the useful findings come from.

## Install

**Claude (web and desktop):**
1. Download [`concept-check.zip`](https://github.com/Halfofthesky/concept-check/releases/latest/download/concept-check.zip).
2. Go to **Customize → Skills → + → Create skill → Upload a skill**.
3. Choose the zip. Code execution must be on in **Settings → Capabilities**.

**Claude Code:** copy the `concept-check/` folder into `~/.claude/skills/`.

**ChatGPT, Gemini or any other model:** the skill is a single plain Markdown file with no scripts. Download [`SKILL.md`](https://github.com/Halfofthesky/concept-check/releases/latest/download/SKILL.md) and paste it into a custom GPT's instructions, a Gem, a project's instructions, or the start of a chat.

## Downloads

From the [latest release](https://github.com/Halfofthesky/concept-check/releases/latest):

| File | For |
|---|---|
| [`concept-check.zip`](https://github.com/Halfofthesky/concept-check/releases/latest/download/concept-check.zip) | Uploading to Claude |
| [`concept-check.skill`](https://github.com/Halfofthesky/concept-check/releases/latest/download/concept-check.skill) | The same archive, `.skill` extension |
| [`SKILL.md`](https://github.com/Halfofthesky/concept-check/releases/latest/download/SKILL.md) | Any other model, as plain text |

## Sources

- John Gerring, "What Makes a Concept Good? A Criterial Framework for Understanding Concept Formation in the Social Sciences," *Polity* 31.3 (1999): 357–393.
- John Gerring, *Social Science Methodology: A Unified Framework*, 2nd ed. (Cambridge University Press, 2012), ch. 5, "Concepts."
- Giovanni Sartori, "Concept Misformation in Comparative Politics," *American Political Science Review* 64.4 (1970): 1033–1053.

The skill merges Gerring's 1999 and 2012 lists and marks the source of each criterion. Adapting it for humanities concepts and for concepts that work in two languages is my own extension. The skill is not affiliated with the authors.

## See also

- [BEAM](https://github.com/Halfofthesky/beam): maps what each source does in your text.
- [Evidence Tests](https://github.com/Halfofthesky/evidence-tests): weighs the evidence for causal claims against rival explanations.
- [Stasis](https://github.com/Halfofthesky/stasis): finds where a disagreement sits and whether the text meets it there.
- [Logic & Reasoning Skills](https://github.com/Halfofthesky/logic-reasoning-skills): reconstructs arguments, spots fallacies, solves formal logic.
- [Adversarial Editorial Review](https://github.com/Halfofthesky/adversarial-editorial-review): three reviewers and an editorial synthesis for humanities manuscripts.

## License

MIT
