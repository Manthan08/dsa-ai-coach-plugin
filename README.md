# DSA AI Coach for Codex

`dsa-ai-coach` is a Codex skill for learning Data Structures and Algorithms with
an attempt-first coaching style.

It is designed for learners who want practical interview preparation without
copying full solutions too early. The skill teaches with short sessions,
story-based explanation, ASCII diagrams, dry runs, C# examples, teach-back
checks, flashcards, and compact revision sheets.

## What It Helps With

- Learning common DSA patterns from beginner level.
- Practicing problems without seeing the final answer first.
- Debugging your own C# DSA code.
- Reviewing a pattern with a concise revision sheet.
- Building long-term recall through flashcards and teach-back checks.

## Install

Add this Codex plugin marketplace:

```powershell
codex plugin marketplace add Manthan08/codex-plugin
```

Then open the Codex plugin directory, select `Manthan08 Codex Skills`, and
install `DSA AI Coach`.

## Use

Start a new Codex thread and ask:

```text
Use $dsa-ai-coach to teach me the next DSA topic without giving full solutions first.
```

You can also ask:

```text
Use $dsa-ai-coach to help me revise two pointers with a compact revision sheet.
```

```text
Use $dsa-ai-coach to debug my C# solution. Give hints before the full fix.
```

## Coaching Style

The skill follows this order by default:

```text
story -> diagram -> dry run -> attempt -> hints -> solution review -> revision
```

It uses C# first and Python only when comparison or simpler syntax helps.

## Included Skill

```text
dsa-ai-coach
```

The skill is packaged as a Codex plugin so it can be installed through a Codex
marketplace.
