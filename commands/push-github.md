---
name: push-github
description: >
  Guidelines for committing and pushing changes to GitHub. Use this whenever
  you are about to make a git commit or push — including after editing files,
  finishing a feature, or fixing a bug. Covers commit message naming conventions
  and branching rules.
---

# push-github

## Branch rule

Always commit and push to **master** (or **main** if that is the default branch name the repo was initialised with). Never create a new branch unless the user explicitly asks for one.

## Commit message format

Follow this pattern:

```
<type>(<scope>): <short description>
```

- **type** — what kind of change this is (see list below)
- **scope** — the file, section, or feature affected (keep it short, e.g. `index`, `nav`, `footer`, `podminky`)
- **short description** — plain English, lowercase, no full stop at the end

### Types

| Type | When to use |
|---|---|
| `feat` | Adding something new (new page, new section, new feature) |
| `fix` | Fixing a bug or broken link |
| `style` | Visual/CSS changes that don't affect content |
| `content` | Text, copy, or translation changes |
| `remove` | Deleting files, sections, or dead code |
| `refactor` | Restructuring code without changing behaviour |
| `docs` | Changes to .md plan files or documentation |

### Examples

| What you did | Commit message |
|---|---|
| Added podminky.html | `feat(podminky): add terms of use page` |
| Removed unconnected nav items | `remove(nav): drop soft skills, certifikace, videokurzy links` |
| Fixed broken link to kurz-clvc | `fix(courses): correct href on VIBE coding card` |
| Updated hero headline text | `content(hero): update CZ headline copy` |
| Tweaked button hover colour | `style(btn): adjust primary button hover yellow shade` |

## Workflow

```bash
# 1. Stage all changed files
git add .

# 2. Commit with a message following the convention above
git commit -m "type(scope): description"

# 3. Push to master
git push origin master
```

If the push is rejected because the remote is ahead, pull first:

```bash
git pull origin master --rebase
git push origin master
```

## Quick checklist before pushing

- [ ] Message follows `type(scope): description` format
- [ ] Description is lowercase and has no trailing full stop
- [ ] Pushing to `master` (not a feature branch)
- [ ] All intended files are staged (`git status` to check)
