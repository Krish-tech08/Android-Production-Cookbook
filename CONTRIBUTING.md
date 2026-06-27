# 🤝 Contributing to Android Production Cookbook

Thank you for taking the time to contribute. This repository exists because developers like you care about raising the quality of Android engineering — and every meaningful contribution helps the next developer learn better.

Please read this document fully before submitting a pull request. It keeps the review process smooth for everyone.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [What We're Looking For](#what-were-looking-for)
- [What to Avoid](#what-to-avoid)
- [Getting Started](#getting-started)
- [Branching Convention](#branching-convention)
- [Commit Message Style](#commit-message-style)
- [Pull Request Process](#pull-request-process)
- [Module Quality Standards](#module-quality-standards)
- [Documentation Standards](#documentation-standards)
- [Reporting Issues](#reporting-issues)
- [Questions](#questions)

---

## 🧭 Code of Conduct

This is a professional, educational, and welcoming space. All contributors are expected to:

- Communicate respectfully in issues, reviews, and discussions
- Give constructive, specific feedback — not vague criticism
- Accept that maintainers may request changes before merging
- Acknowledge that disagreements about implementation are normal and should be resolved with reasoning, not frustration

Disrespectful behavior of any kind will result in removal from the project.

---

## ✅ What We're Looking For

Contributions that align with the repository's goal of **production-quality Android engineering** are always welcome. Specifically:

- 🐛 **Bug fixes** — Incorrect implementations, outdated APIs, deprecated usage
- 📝 **Documentation improvements** — Clearer explanations, better inline comments, corrected references
- ➕ **New production patterns** — Real-world approaches to problems not yet covered in existing modules
- 🔗 **Reference additions** — Links to relevant official Android documentation, talks, or blog posts from credible sources
- 🧪 **Test coverage** — Unit tests, ViewModel tests, or UI tests for existing module code
- ♻️ **Refactors** — Improvements to code clarity, naming, or structure without changing behavior

---

## ❌ What to Avoid

To maintain the repository's standard, the following will not be accepted:

- ❌ Tutorial-style code with no architectural context
- ❌ Incomplete implementations left as "exercises for the reader"
- ❌ Code copied directly from official documentation samples without production adaptation
- ❌ Undocumented patterns with no explanation of why the approach was chosen
- ❌ Contributions that introduce dependencies without justification
- ❌ Unformatted code or code that doesn't follow the existing module structure
- ❌ PRs that modify multiple unrelated modules at once

When in doubt, open an issue first and discuss before building.

---

## 🚀 Getting Started

### 1. Fork the Repository

Click **Fork** at the top right of this repository page to create your own copy.

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/android-production-cookbook.git
cd android-production-cookbook
```

### 3. Add the Upstream Remote

```bash
git remote add upstream https://github.com/krishkumarchaurasia/android-production-cookbook.git
```

### 4. Keep Your Fork in Sync

Before starting any work, always pull the latest changes from upstream:

```bash
git fetch upstream
git checkout main
git merge upstream/main
```

---

## 🌿 Branching Convention

Always create a new branch for your contribution. Never work directly on `main`.

| Type | Branch Format | Example |
|---|---|---|
| New module | `module/topic-name` | `module/foreground-services` |
| Bug fix | `fix/short-description` | `fix/room-migration-crash` |
| Documentation | `docs/short-description` | `docs/hilt-module-explanation` |
| Refactor | `refactor/short-description` | `refactor/retrofit-error-handling` |

```bash
git checkout -b module/your-topic-name
```

---

## ✍️ Commit Message Style

Write commit messages that explain *what changed and why*, not just *what you did*.

**Format:**

```
type(scope): short summary in present tense

Optional body explaining the reasoning behind the change.
```

**Types:**

| Type | When to Use |
|---|---|
| `feat` | Adding a new module or pattern |
| `fix` | Correcting a bug or incorrect implementation |
| `docs` | Documentation-only changes |
| `refactor` | Code restructure without behavior change |
| `test` | Adding or improving tests |
| `chore` | Build config, Gradle, or tooling changes |

**Examples:**

```
feat(room): add migration strategy with fallback example

fix(hilt): correct ViewModel injection scope in multi-module setup

docs(coroutines): clarify structured concurrency explanation in README
```

---

## 📬 Pull Request Process

### Before Submitting

- [ ] Your branch is up to date with `upstream/main`
- [ ] Code compiles without errors or warnings
- [ ] Kotlin style follows the existing codebase conventions
- [ ] All new code has inline comments explaining non-obvious decisions
- [ ] The module's `README.md` is updated or created if adding a new module
- [ ] No unrelated files are included in the PR

### PR Title Format

```
[Module Name] Short description of what this PR does
```

Examples:
```
[Room] Add type converter examples for complex objects
[Hilt] Fix incorrect scoping in ViewModel injection example
[Docs] Improve coroutines dispatcher explanation
```

### PR Description Template

When opening a pull request, include the following:

```markdown
## What does this PR do?
A clear, one-paragraph description of the change.

## Why is this needed?
Explain the problem this solves or the gap it fills.

## What production scenario does this address?
Describe a real-world situation where this pattern or fix would apply.

## Screenshots (if applicable)
Include before/after or output screenshots for UI-related changes.

## Checklist
- [ ] Code compiles and runs correctly
- [ ] Inline comments explain non-obvious decisions
- [ ] Module README is updated
- [ ] No unrelated changes included
```

### Review Process

- A maintainer will review your PR within a reasonable timeframe
- You may be asked to make changes before merging — this is normal and not a rejection
- Once approved, your contribution will be merged into `main`

---

## 📐 Module Quality Standards

Every module in this repository should meet the following bar:

### Code
- Written in idiomatic Kotlin — no Java-style patterns
- Follows MVVM or Clean Architecture conventions where applicable
- Uses Jetpack Compose for UI where a UI is involved
- No hardcoded strings, magic numbers, or unexplained constants
- Error cases are handled explicitly — no silent failures

### Structure
Every module folder should contain:

```
XX-Module-Name/
├── README.md          ← Concept overview, why it exists, best practices, common mistakes
├── src/
│   ├── data/          ← Repository, data source, models
│   ├── domain/        ← Use cases, interfaces
│   └── presentation/  ← ViewModel, UI state, Composables
└── screenshots/       ← Optional, for UI modules
```

### Documentation
- Every public function and class should have a KDoc comment
- Non-obvious implementation decisions must have an inline comment explaining the *why*
- The module `README.md` must include a section on common mistakes

---

## 📝 Documentation Standards

When writing or improving documentation:

- Write for someone encountering this topic for the second or third time — not the very first time, and not an expert
- Explain the *reason* behind a pattern, not just the syntax
- Use short paragraphs over long walls of text
- Use code blocks for all code snippets, with the language specified (` ```kotlin `)
- Link to official Android documentation when referencing APIs or components

---

## 🐞 Reporting Issues

If you find a bug, outdated implementation, or incorrect explanation, please open an issue before submitting a fix.

**A good issue includes:**

- The module and file name where the problem exists
- What the current behavior or explanation is
- What the correct behavior or explanation should be
- A reference to official documentation if applicable

Use the issue title format:
```
[Module Name] Short description of the problem
```

---

## 💬 Questions

If you are unsure whether your contribution is a good fit, open a **Discussion** before spending time building it. It is always better to align on scope and direction early.

---

<div align="center">

*Every contribution — no matter how small — moves this resource forward for the next developer who needs it.*

**Thank you for contributing.**

</div>
