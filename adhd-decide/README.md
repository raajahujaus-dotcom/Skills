# adhd-decide

Structured decision support for people with ADHD. Type `/adhd-decide` followed by the decision you're stuck on.

## What it does

- Starts helping right away instead of asking a list of questions first
- Classifies the decision by how reversible and costly it is
- Separates facts from interpretations and assumptions
- Offers three options at most
- Ends with one next step that takes 5-20 minutes, plus one decision rule with a date
- Treats late-night or anxious urgency as a reason to pause, not to decide

## When it runs

Only when you type `/adhd-decide`. It stays out of ordinary advice questions on purpose.

## Example

```
/adhd-decide I can't decide between two laptops. I've researched for two weeks.
```

Expected shape of the reply: a one-sentence restatement of the decision, a decision type with a reason, facts vs. interpretations, up to three options, a timed next step, and a decision rule with a date.

## What it won't do

- Diagnose ADHD, anxiety, or any other condition
- Give medical, medication, legal, or financial instructions
- Replace professional support. It points toward it when symptoms are impairing or there is any safety concern.

## Files

- `SKILL.md`: the skill itself
- `evals/evals.json`: sample test prompts
