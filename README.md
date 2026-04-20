# Flutter Agent Skills

The most complete Flutter agent skill set for AI coding assistants.
Covers every app type, stack, state management, backend, and technology
a Flutter developer needs — for any app, any platform, any stack.

Built and maintained by [Md Azad Hossain Tutul](https://github.com/mdazadhossain95) —
Flutter developer with 5+ years of experience and 200+ apps shipped.

## Installation

To install all skills into your project, run:

```bash
npx skills add mdazadhossain95/flutter-agent-skills
```

## Updating Skills

```bash
npx skills update mdazadhossain95/flutter-agent-skills
```

## How To Use Skills

After installing, ask your AI coding assistant for a specific task in natural language. The assistant will match your request to the right skill.

### Quick Start

1. Open your Flutter project in your AI-enabled editor.
2. Install skills:

```bash
npx skills add mdazadhossain95/flutter-agent-skills
```

3. Ask for what you want to build.

### Example Prompts

- "Set up Flutter app architecture with UI, logic, and data layers."
- "Create a Flutter form with validation and error messages."
- "Implement deep-linking navigation for a Flutter app."
- "Add local database support and repository pattern in Flutter."
- "Use flutter-project-bootstrap and scaffold an ecommerce starter app."

### Using The Bootstrap Skill

Use [flutter-project-bootstrap](skills/flutter-project-bootstrap/SKILL.md) when you want fast project scaffolding.

The bootstrap flow supports:

- Guided mode: asks questions (app type, state management, backend, push, auth, etc.) and scaffolds from your answers.
- Quick default mode: skips questions and generates a recommended starter stack.

Example bootstrap prompts:

- "Run flutter-project-bootstrap in guided mode."
- "Run flutter-project-bootstrap in quick mode for an ecommerce app."
- "Bootstrap a rider app with Bloc, REST API, and Firebase push notifications."

### Best Practice

- Start with one clear request.
- Confirm generated structure before adding advanced features.
- Add new features step-by-step (auth, payments, realtime, analytics).
- Re-run update periodically to keep skills current.

---

## Available Skills

### 📦 Official Flutter Skills

> Originally from [flutter/skills](https://github.com/flutter/skills) by the Flutter team.
> Copyright 2026 The Flutter Authors. Licensed under [BSD-3-Clause](LICENSE-flutter-skills).

| Skill | Description |
|---|---|
| [flutter-adding-home-screen-widgets](skills/flutter-adding-home-screen-widgets/SKILL.md) | Adds home screen widgets to a Flutter app for Android and iOS. Use when providing glanceable app information or quick actions on the device home screen. |
| [flutter-animating-apps](skills/flutter-animating-apps/SKILL.md) | Implements animated effects, transitions, and motion in a Flutter app. Use when adding visual feedback, shared element transitions, or physics-based animations. |
| [flutter-architecting-apps](skills/flutter-architecting-apps/SKILL.md) | Architects a Flutter application using the recommended layered approach (UI, Logic, Data). Use when structuring a new project or refactoring for scalability. |
| [flutter-building-forms](skills/flutter-building-forms/SKILL.md) | Builds Flutter forms with validation and user input handling. Use when creating login screens, data entry forms, or any multi-field user input. |
| [flutter-building-layouts](skills/flutter-building-layouts/SKILL.md) | Builds Flutter layouts using the constraint system and layout widgets. Use when creating or refining the UI structure of a Flutter application. |
| [flutter-building-plugins](skills/flutter-building-plugins/SKILL.md) | Builds Flutter plugins that provide native interop for other apps to use. Use when creating reusable packages that bridge Flutter with platform-specific functionality. |
| [flutter-caching-data](skills/flutter-caching-data/SKILL.md) | Implements caching strategies for Flutter apps to improve performance and offline support. Use when retaining app data locally to reduce network requests or speed up startup. |
| [flutter-embedding-native-views](skills/flutter-embedding-native-views/SKILL.md) | Embeds native Android, iOS, or macOS views into a Flutter app. Use when integrating complex native components like maps or web views. |
| [flutter-handling-concurrency](skills/flutter-handling-concurrency/SKILL.md) | Executes long-running tasks in background isolates to keep the UI responsive. Use when performing heavy computations or parsing large datasets. |
| [flutter-handling-http-and-json](skills/flutter-handling-http-and-json/SKILL.md) | Executes HTTP requests and handles JSON serialization in a Flutter app. Use when integrating with REST APIs or parsing structured data from external sources. |
| [flutter-implementing-navigation-and-routing](skills/flutter-implementing-navigation-and-routing/SKILL.md) | Handles routing, navigation, and deep linking in a Flutter application. Use when moving between screens or setting up URL-based navigation. |
| [flutter-improving-accessibility](skills/flutter-improving-accessibility/SKILL.md) | Configures a Flutter app to support assistive technologies like Screen Readers. Use when ensuring an application is usable for people with disabilities. |
| [flutter-interoperating-with-native-apis](skills/flutter-interoperating-with-native-apis/SKILL.md) | Interoperates with native platform APIs on Android, iOS, and the web. Use when accessing device-specific features not available in Dart or calling existing native code. |
| [flutter-localizing-apps](skills/flutter-localizing-apps/SKILL.md) | Configures a Flutter app to support multiple languages and regions. Use when preparing an application for international markets and diverse user locales. |
| [flutter-managing-state](skills/flutter-managing-state/SKILL.md) | Manages application and ephemeral state in a Flutter app. Use when sharing data between widgets or handling complex UI state transitions. |
| [flutter-reducing-app-size](skills/flutter-reducing-app-size/SKILL.md) | Measures and optimizes the size of Flutter application bundles for deployment. Use when minimizing download size or meeting app store package constraints. |
| [flutter-setting-up-on-linux](skills/flutter-setting-up-on-linux/SKILL.md) | Sets up a Linux environment for Flutter development. Use when configuring a Linux machine to run, build, or deploy Flutter applications. |
| [flutter-setting-up-on-macos](skills/flutter-setting-up-on-macos/SKILL.md) | Sets up a macOS environment for Flutter development. Use when configuring a macOS machine to run, build, or deploy Flutter applications for iOS or macOS. |
| [flutter-setting-up-on-windows](skills/flutter-setting-up-on-windows/SKILL.md) | Sets up a Windows environment for Flutter development. Use when configuring a Windows machine to run, build, or deploy Flutter applications for Windows desktop or Android. |
| [flutter-testing-apps](skills/flutter-testing-apps/SKILL.md) | Implements unit, widget, and integration tests for a Flutter app. Use when ensuring code quality and preventing regressions through automated testing. |
| [flutter-theming-apps](skills/flutter-theming-apps/SKILL.md) | Customizes the visual appearance of a Flutter app using the theming system. Use when defining global styles, colors, or typography for an application. |
| [flutter-working-with-databases](skills/flutter-working-with-databases/SKILL.md) | Manages local data persistence using SQLite or other database solutions. Use when a Flutter app needs to store, query, or synchronize large amounts of structured data on the device. |

---

### 🚀 Extended Skills

> Created and maintained by [Md Azad Hossain Tutul](https://github.com/mdazadhossain95).
> Licensed under [MIT](LICENSE).

| Skill | Description |
|---|---|
| [flutter-project-bootstrap](skills/flutter-project-bootstrap/SKILL.md) | Scaffolds a Flutter app structure from developer requirements. Supports a guided questionnaire and a quick default mode, then generates architecture, dependencies, starter files, and 1-2 sample screens. |
| [flutter-explain-codebase](skills/flutter-explain-codebase/SKILL.md) | Explains a Flutter project codebase in a structured, developer-friendly way, including architecture, state management, data flow, navigation, dependencies, risks, and prioritized next actions. |
| [flutter-optimize-codebase](skills/flutter-optimize-codebase/SKILL.md) | Optimizes a Flutter codebase for performance, maintainability, architecture quality, and release readiness using a prioritized, evidence-driven improvement plan. |

---

## Contributing

Have an idea for a new skill? Found a bug or improvement?

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute.

New skills are added based on:
- Real developer needs and questions
- New popular Flutter packages
- New app types and use cases
- Community requests via GitHub Issues

---

## Licenses

- **Extended skills** (created by this repo) → [MIT License](LICENSE) — Copyright 2026 Md Azad Hossain Tutul
- **Official Flutter skills** → [BSD-3-Clause License](LICENSE-flutter-skills) — Copyright 2026 The Flutter Authors

---

## Code of Conduct

Please see [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for more information.