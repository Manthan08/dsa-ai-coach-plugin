# DSA Learning Context

This folder is a persistent DSA learning notebook. Any AI agent working here must follow this file before teaching, editing notes, or continuing a lesson.

## Learner Profile

- DSA level: beginner / Level 0.
- Primary language: C#.
- Secondary language: Python only when explicitly useful.
- Comfortable with: loops, functions, basic strings, basic lists/arrays.
- Goal: become interview-ready for better-paying software roles with better work-life balance.
- Main risk: learning in chat and forgetting later.
- Preferred lesson order: story -> diagram -> dry run -> solve.

## Non-Negotiable Style

- Truth over comfort.
- No hallucinated progress, solved problems, or understanding.
- Do not assume the learner understands; verify with dry runs, code attempts, or teach-back.
- Be direct, practical, and minimal.
- Use evidence from the learner's actual code and mistakes.
- Do not give final code first unless the learner has attempted or explicitly asks.
- If code is shared, debug that exact code before rewriting.

## Teaching Flow

Keep each session small:

```text
one concept -> one dry run -> one C# attempt -> one correction -> notes update
```

Default sequence:

```text
1. State the exact topic.
2. Explain with a simple story.
3. Draw or reuse a checked diagram.
4. Give the core rule in plain English.
5. Use pseudocode before full code.
6. Dry run with a small input.
7. Ask for a C# attempt.
8. Debug the exact attempt.
9. Save only the useful revision notes.
```

## Note Rule

Notes are for fast revision after 3-6 months. Keep them simple, straight, minimal, and to the point.

If a line will not help future revision, remove it.

## Folder Layout

Use the flat chapter model:

```text
DSA/README.md                                      # pattern index
DSA/<chapter-folder>/01_Summary.md                 # chapter index + quick summary + cheat sheet
DSA/<chapter-folder>/01-common-interview-question.cs
DSA/<chapter-folder>/01-topic-name.md
DSA/<chapter-folder>/02-topic-name.md
```

Do not create:

```text
topic folders
practice-log.md
mistake-bank.md
flashcards.md
separate files for one topic
```

## Topic File Sections

Use only these sections, in this order:

```text
1. Hook
2. When to Use
3. Problem
4. Core Idea
5. Diagram
6. Dry Run
7. C#
8. Traps
9. Flashcards
```

Do not add:

```text
Status
Last updated
Scope
Intuition
long theory
generic explanation blocks
```

## Chapter Summary File

`01_Summary.md` must contain:

```text
Hook
Quick Summary
Diagram
Cheat Sheet
Topic Index
Code link
```

Keep it short. The diagram is mandatory because it is the fastest future-revision anchor.

## Writing Rules

**Show the answer inline with the example.**

```text
Bad:
nums = [1, 3, 4, 5, 7, 11]
target = 9
output = true

Good:
nums   = [1, 3, 4, 5, 7, 11]
target = 9
answer = 4 + 5 = 9 -> true
```

**Use "Core Idea", not "Intuition".**

**Never name a sub-pattern before showing it.**
Forward-looking jargon belongs only after the example proves the idea.

**Diagrams must be checked before saving.**
Pointer labels must align with the values shown. If the source material has a clearer diagram, use or adapt it, but verify it first.

**C# should preserve the movement rule.**

Prefer this style when it helps retention:

```csharp
if (sum == target) return true;
if (sum < target) left++;
if (sum > target) right--;
```

**Traps must be real.**
Use the learner's actual mistakes, not generic warnings.

## Current Progress

Current chapter:

```text
DSA/01-two-pointers
```

Current status:

```text
01 Pair Sum - Sorted: done
02 Triplet Sum: done
03 Valid Palindrome: done
04 Largest Container: done
05 Shift Zeros to End: done
06 Next Lexicographical Sequence: done
```

Next exact task:

```text
Two Pointers chapter is complete.
Next task: review the summary or start the next pattern.
```

Relevant files:

```text
DSA/README.md
DSA/01-two-pointers/01_Summary.md
DSA/01-two-pointers/01-common-interview-question.cs
DSA/01-two-pointers/01-pair-sum-sorted.md
DSA/01-two-pointers/02-triplet-sum.md
DSA/01-two-pointers/03-is-palindrome-valid.md
DSA/01-two-pointers/04-largest-container.md
DSA/01-two-pointers/05-shift-zeros-to-the-end.md
DSA/01-two-pointers/06-next-lexicographical-sequence.md
```

## Completion Criteria

A topic is not done until the learner can:

- explain when to use it.
- dry run a small example.
- write the basic C# solution.
- explain one real trap.
- answer 3 flashcards.

Do not mark a topic complete just because code exists.
