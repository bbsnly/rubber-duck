# rubber-duck 🦆

An agent skill that turns your coding agent into a rubber duck. It asks the
questions that lead you to your own answer and does not hand the answer over.

Use it when you are stuck on a bug, a design, a decision or an argument that
won't come together, and you would learn more from finding the answer than from
being told it.

## Install

With the [`skills`](https://skills.sh) CLI, for any agent that supports
[Agent Skills](https://agentskills.io):

```bash
npx skills add bbsnly/rubber-duck
```

As a Claude Code plugin:

```bash
claude plugin marketplace add bbsnly/rubber-duck
claude plugin install bbsnly@bbsnly
```

## Use

Ask for it in your own words:

```text
rubber duck me: this function drops the last item and I can't see why
```

```text
I want to think out loud about whether to take this job offer
```

In Claude Code you can also call it directly with `/bbsnly:rubber-duck`.

## What to expect

- **Questions, not answers.** At most two per turn, then it waits for you.
- **Facts when you need them.** If you are missing a fact, such as what an error
  message means, it tells you, then goes back to asking.
- **No verdicts.** It will not name the bug or make the decision for you.
- **A way out.** Say "just tell me" and it checks once that you mean it, then
  answers directly and in full.

## Example

> **You:** rubber duck me. `total([1, 2, 3])` gives 3, I expected 6.
>
> **Duck:** Walk through it slowly. What does `range(len(nums) - 1)` produce,
> exactly? Write out the values of `i` it hands you.

## License

[MIT](LICENSE)
