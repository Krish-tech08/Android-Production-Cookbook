<div align="center">

# 🍳 Android Production Cookbook

**A collection of production-ready Android engineering examples, patterns, architectures, and best practices built with Kotlin and Jetpack Compose.**

<br/>

[![Kotlin](https://img.shields.io/badge/Kotlin-2.0-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-Latest-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Android](https://img.shields.io/badge/Android-API%2026+-3DDC84?style=flat-square&logo=android&logoColor=white)](https://developer.android.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)
[![Stars](https://img.shields.io/github/stars/vidagdhan/android-production-cookbook?style=flat-square)](https://github.com/vidagdhan/android-production-cookbook/stargazers)

<br/>

<img src="https://developer.android.com/static/images/logos/android.svg" width="80" alt="Android Logo"/>

</div>

---

## 📖 What Is This?

Most Android tutorials teach you *what* to build. This repository focuses on *how production systems are built* — and more importantly, *why* they are designed the way they are.

The **Android Production Cookbook** is designed to bridge the gap between beginner tutorials and real-world Android applications. Every module in this repository demonstrates how common features are implemented in production apps, with scalability, maintainability, and clean architecture in mind.

This is not a sample app. It is a **structured reference repository** — a collection of independently organized modules that professional engineers, students, and career-changers can study, adapt, and apply directly in their own projects.

> Each module addresses a specific domain of Android development: from project setup and dependency injection to background work, testing, security, and CI/CD pipelines. The goal is always the same: understand the reasoning behind the implementation, not just the syntax.

---

## 👩‍💻 Who Is This For?

This repository is useful regardless of where you are in your Android journey.

| Audience | How This Helps |
|---|---|
| 🌱 **Android Beginners** | See how real apps structure code from day one |
| 🔧 **Intermediate Developers** | Move from "it works" to "it scales" |
| 🎓 **Students Preparing for Internships** | Build portfolio-worthy understanding of production patterns |
| 💼 **Professional Android Engineers** | Use as a reference for architecture decisions and patterns |
| ☕ **Java-to-Kotlin Transitioning Devs** | See idiomatic Kotlin applied across all layers |
| 🧭 **Anyone Wanting Production-Level Practices** | Learn the industry standard, not just the basics |

---

## 🗂️ Repository Structure

```
Android-Production-Cookbook
│
├── 01-Project-Setup
├── 02-MVVM
├── 03-Clean-Architecture
├── 04-Hilt-DI
├── 05-Room-Database
├── 06-Retrofit
├── 07-Coroutines
├── 08-StateFlow
├── 09-Compose-Navigation
├── 10-WorkManager
├── 11-Foreground-Services
├── 12-Notifications
├── 13-Firebase
├── 14-Play-Billing
├── 15-Paging3
├── 16-CameraX
├── 17-Permissions
├── 18-Offline-First
├── 19-Testing
├── 20-Performance
├── 21-Security
├── 22-CI-CD
│
└── README.md
```

Each folder is a self-contained module. You can study them in order or jump directly to the topic you need.

---

## 📦 What Each Module Contains

Every module is structured to give you complete context — not just code.

<details>
<summary><strong>Click to expand module structure</strong></summary>

<br/>

| Section | Description |
|---|---|
| 📝 **Concept Overview** | A plain-language explanation of what this topic is and where it fits in an Android app |
| 🤔 **Why It Exists** | The problem it solves and why the Android team or community adopted this approach |
| 🏗️ **Production Implementation** | Clean, annotated Kotlin code showing how this is done in a real app |
| 🧱 **Clean Architecture Integration** | How this module fits into the data/domain/presentation layer separation |
| ✅ **Best Practices** | Patterns that experienced engineers follow in production codebases |
| ⚠️ **Common Mistakes** | Anti-patterns, memory leaks, race conditions, and other pitfalls to avoid |
| 🖼️ **Screenshots** | Visual output where applicable |
| 📁 **Folder Structure** | How files are organized within a real feature package |
| 📚 **References** | Links to official Android documentation, architecture guides, and related resources |

</details>

---

## 🛠️ Technologies Covered

<details>
<summary><strong>Language & Core</strong></summary>

- **Kotlin** — Idiomatic Kotlin across all modules (coroutines, extension functions, sealed classes, data classes)
- **Jetpack Compose** — Declarative UI with state management, theming, and reusable components
- **Material 3** — Design tokens, adaptive layouts, and component usage following M3 guidelines

</details>

<details>
<summary><strong>Architecture & Dependency Injection</strong></summary>

- **MVVM** — ViewModel, LiveData, StateFlow, and the unidirectional data flow pattern
- **Clean Architecture** — Data / Domain / Presentation layer separation with use cases and repositories
- **Hilt** — Compile-time dependency injection, scoping, and module organization

</details>

<details>
<summary><strong>Async, Data & Networking</strong></summary>

- **Coroutines** — Structured concurrency, exception handling, and dispatcher selection
- **Flow / StateFlow / SharedFlow** — Reactive streams for UI state and one-time events
- **Room** — Local database with DAOs, migrations, and type converters
- **Retrofit** — REST API integration with sealed result wrappers and error handling
- **Paging 3** — Efficient large data set loading with remote mediators

</details>

<details>
<summary><strong>Background Work & System Integration</strong></summary>

- **WorkManager** — Reliable background tasks with constraints and chaining
- **Foreground Services** — Long-running tasks with proper lifecycle and notification binding
- **Notifications** — Channels, groups, deep links, and notification actions
- **CameraX** — Camera capture, analysis pipelines, and lifecycle-aware integration

</details>

<details>
<summary><strong>Firebase & Billing</strong></summary>

- **Firebase** — Authentication, Firestore, Realtime Database, Cloud Messaging, and Crashlytics
- **Play Billing** — One-time purchases, subscriptions, purchase verification, and billing client lifecycle

</details>

<details>
<summary><strong>Testing & Quality</strong></summary>

- **JUnit** — Unit testing for ViewModels, use cases, and repositories
- **MockK** — Kotlin-first mocking library for writing expressive test doubles
- **Compose Testing** — Semantic tree testing, state-driven UI tests, and navigation testing

</details>

<details>
<summary><strong>DevOps & Performance</strong></summary>

- **GitHub Actions** — CI/CD pipelines for build, lint, test, and Play Store deployment
- **Performance** — Baseline Profiles, App Startup, memory profiling, recomposition analysis
- **Security** — Certificate pinning, EncryptedSharedPreferences, ProGuard rules, and API key handling

</details>

---

## 🎯 Repository Goals

This repository is built around a set of deliberate engineering goals:

- **Learn Android the production way** — Build habits that scale beyond tutorial-sized projects
- **Build maintainable apps** — Write code your future self (and teammates) can navigate
- **Understand architecture instead of memorizing code** — Know *why* a pattern exists before applying it
- **Improve debugging skills** — Learn how to diagnose, isolate, and fix real-world problems
- **Follow modern Android development practices** — Stay aligned with the direction the Android platform is actively moving toward
- **Prepare for internships and real-world development** — Build the contextual knowledge that tutorials leave out

---

## 🗺️ Recommended Learning Path

If you are starting from scratch or want a structured progression, follow this order:

```
1.  📁  Project Setup          →  Build configs, Gradle structure, product flavors
2.  🔤  Kotlin Fundamentals    →  Idiomatic Kotlin patterns used across all modules
3.  🎨  Jetpack Compose        →  UI state, recomposition, theming, component design
4.  🧭  Compose Navigation     →  NavHost, arguments, deep links, bottom nav
5.  🏛️  MVVM                   →  ViewModel, StateFlow, UI state modeling
6.  💉  Hilt DI                →  Modules, bindings, scopes, ViewModel injection
7.  🗄️  Room Database          →  Entities, DAOs, migrations, relationships
8.  🌐  Retrofit               →  API layer, error handling, sealed response wrappers
9.  ⚡  Coroutines & Flow      →  Async patterns, cancellation, error propagation
10. ⚙️  WorkManager            →  Background work, chaining, periodic tasks
11. 🔥  Firebase               →  Auth, Firestore, FCM, Crashlytics
12. 🚀  Performance            →  Profiling, startup, Baseline Profiles
13. 🧪  Testing                →  Unit, integration, and UI tests
14. 🔄  CI/CD                  →  Automated build, lint, test, and release pipelines
```

> **Note:** Modules are independent. You can jump to any topic at any time — the path above is a suggestion, not a requirement.

---

## 🤝 Contributing

Contributions are welcome and appreciated. This repository grows through the collective effort of developers who care about the quality of the Android ecosystem.

**Ways to contribute:**

- 📝 Improve or expand existing module documentation
- 🐛 Fix incorrect implementations or outdated API usage
- ➕ Add new production patterns or architectural examples
- 💬 Enhance inline code comments for clarity
- 🔗 Add references to relevant official documentation or talks

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request. All contributions should align with the production-quality standard this repository maintains.

---

## 📄 License

```
MIT License

Copyright (c) 2024 Krish Kumar Chaurasia

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

See [LICENSE](LICENSE) for the full text.

---

<div align="center">

### ⭐ If this repository helps you grow as an engineer, consider giving it a star.

It helps other developers find this resource.

<br/>

---

*"Great Android apps aren't built by copying tutorials — they're built by understanding why production systems are designed the way they are."*

<br/>

**Made with care by [Vidagdhan Technologies](https://github.com/vidagdhan)**

</div>
