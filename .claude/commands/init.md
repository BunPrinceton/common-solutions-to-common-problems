# Common Solutions to Common Problems - Init

You are helping maintain a repository of fixes for things that should be easy but are dumb for no reason.

## Repository Structure

```
common-solutions-to-common-problems/
├── README.md
├── printers/
├── bluetooth/
├── windows/
├── audio/
├── networking/
└── [other categories as needed]/
```

## When Adding a New Solution

Use this template:

```markdown
# [Problem Title]

**Device/Software:** [What this applies to]
**Problem:** [One-line description]
**Date Fixed:** [YYYY-MM-DD]

## Symptoms

- [What you see happening]
- [Error messages if any]

## Things That DON'T Work

- [What you tried that failed]
- [Save others the frustration]

## The Actual Fix

[Step-by-step solution that actually works]

## Why This Happens

[Brief explanation if known]

## Time Wasted Before Finding Fix

[Be honest lol]

## Time To Fix Once You Know

[Usually way shorter]
```

## Categories

Add new categories as needed. Common ones:
- `printers/` - Printer driver hell
- `bluetooth/` - Pairing nightmares
- `windows/` - Windows being Windows
- `audio/` - Sound issues
- `networking/` - WiFi, DNS, etc.
- `software/` - Specific app fixes
- `hardware/` - Physical device issues

## Your Task

Ask the user:
1. What problem did you just solve?
2. What category does it fit in?
3. Walk me through what finally worked

Then create the solution file following the template.
