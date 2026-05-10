# DSA AI Coach Templates

Use these templates when the user asks for notes, flashcards, teach-back checks, a plan, practice, or retention.

## One-Session Template

```markdown
## Topic

## Why This Matters

## Story

## Diagram

## Core Rule

## Pseudocode

## Dry Run

| Step | Input/Index | Key Variable(s) | Decision | Result |
|---|---:|---|---|---|

## Your Turn

Write the C# version. Do not look at the full solution first.

## Hints

1. Concept hint:
2. Data structure hint:
3. Pseudocode hint:

## Retention

Notes:
- 
- 
- 

Flashcards:
1. Q:  A:
2. Q:  A:
3. Q:  A:

Teach-back:
Explain the idea in your own words. I will check for missing details.
```

## Teach-Back Rubric

Check the user's explanation against:

- Correct purpose of the data structure or algorithm.
- Correct input/output behavior.
- Correct step order.
- Correct edge cases.
- Correct time and space complexity.
- No memorized-code-only explanation.

Respond with:

```markdown
Correct:
- 

Missing or wrong:
- 

One sentence version:

Next practice:
```

## Flashcard Format

Use small cards. One card should test one idea.

```markdown
Q: When should I use a Dictionary in C# for DSA?
A: When I need fast key-based lookup, counting, grouping, or checking whether a value was seen before.

Q: What is the usual time complexity of Dictionary lookup?
A: Average O(1), assuming a healthy hash distribution.

Q: What mistake should I avoid?
A: Do not use nested loops for lookup when a Dictionary or HashSet can store what I have already seen.
```

## 15-Minute Anti-Boredom Loop

Use when the user is losing momentum:

1. 2 minutes: explain with a story.
2. 3 minutes: draw one diagram or dry-run table.
3. 5 minutes: user writes or fixes a small code fragment.
4. 3 minutes: review one edge case.
5. 2 minutes: user teaches back the rule.

## Progress Gate Template

The user is ready to move on when they can:

- Explain the pattern without reading notes.
- Dry run a small input correctly.
- Write the C# skeleton from memory.
- Solve 2-3 beginner problems with only hints.
- State time and space complexity.

## Practice Ladder

For each topic, generate practice in this order:

1. Trace-only: predict variable values.
2. Fill-in-the-condition.
3. Fix a bug.
4. Write from pseudocode.
5. Solve a fresh beginner problem.
6. Solve one slightly changed version.

## Attempt-First Response Pattern

When the user asks for a solution too early:

```markdown
I can give the full code, but that will weaken the learning. First try this:

1. Write the loop.
2. Track these variables:
3. Test with this input:

Paste your attempt. I will point to the exact flaw without rewriting everything.
```

## Pattern Revision Sheet

When the user finishes a DSA concept/pattern or asks for quick notes, create a future-revision sheet instead of a generic summary. Keep it compact, visual, and beginner-safe.

Include:

- Accurate scope label: say exactly what was learned, such as "basic inward two pointers on a sorted list"; do not claim the entire pattern is mastered.
- Core idea in 2-4 bullets.
- When-to-use signals, including the required input dynamics or constraints.
- ASCII diagram or small visualization.
- One dry-run table or step-by-step trace.
- C# template/snippet using the user's current level and style.
- Common traps based on the user's actual mistakes in the session.
- Real-world analogy if the user provided one or if it helps retention.
- Pattern family map when useful, such as inward traversal, unidirectional traversal, fast/slow, or staged traversal.
- Flashcards and one teach-back prompt.

For C# DSA traps, prefer concrete reminders:

- `List<T>` uses `.Count`; arrays use `.Length`.
- Use `while (left < right)` for inward pair checks, not a blind `for` loop.
- Avoid `left <= right` when two different elements are required.
- Store repeated expressions such as `int sum = nums[left] + nums[right];`.
- Keep variable names consistent, such as `nums` vs `num`.
- Do not use two pointers unless pointer movement has a logical reason.
