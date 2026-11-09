# SwiftUI Engineering — Agent Skill

An agent skill that guides AI coding assistants to act as senior SwiftUI engineers and interface architects — building, debugging, and refining native Apple user interfaces with declarative UI, state management, navigation, accessibility, and modern Apple design conventions.

**Skill name:** `swiftui-engineering`
**Trigger description:** Build, debug, and refine native SwiftUI interfaces using declarative UI, state management, navigation, reusable components, accessibility, and modern Apple design conventions. Use when building, reviewing, refactoring, or debugging SwiftUI views and interfaces.

---

## What It Does

When loaded into an AI coding assistant (Manus, Claude Code, Cursor, Codex, OpenCode, and others that support the agent skill format), this skill enforces professional SwiftUI engineering discipline:

- **Declarative native UI first** — native SwiftUI components, layouts, materials, and system behaviors over web-based or cross-platform imitations.
- **Clean view architecture** — small reusable views, lean `body` declarations, business logic kept outside views, and appropriate use of `@ViewBuilder`, `Grid`, `List`, and lazy containers.
- **State management discipline** — the right state primitive for the project's OS version (`@Observable`, `@State`, `@Binding`, `@Environment`, `@StateObject`), single sources of truth, computed derived values, and concurrency-safe updates.
- **Robust navigation and UX** — `NavigationStack`/`NavigationSplitView`, typed routes, explicit loading/empty/error states, duplicate-submission guards, and preserved navigation state.
- **Apple design conventions** — Light/Dark mode support, semantic system colors, SF Symbols, purposeful animations respecting Reduce Motion, and consistent visual hierarchy.
- **Accessibility by default** — VoiceOver labels and hints, Dynamic Type, sufficient contrast, usable hit targets, and keyboard friendliness.
- **Performance awareness** — expensive work kept out of `body`, stable `ForEach` identifiers, and claims verified with Instruments rather than guessed.
- **Honest verification** — inspecting existing conventions before editing, checking Xcode builds/previews/simulator when available, and never claiming unverified success.

---

## Installation

### Manus

1. Open Manus → **Settings → Skills**.
2. Click **Import from GitHub** and enter:
   ```
   https://github.com/mshanghai570/swiftui-engineering-agent-skill-
   ```
3. Or import directly with one click:
   **[Import to Manus](https://manus.im/app#settings/skills/import?githubUrl=https://github.com/mshanghai570/swiftui-engineering-agent-skill-)**

### Claude Code / Codex / OpenCode (`npx skills`)

```bash
npx skills add mshanghai570/swiftui-engineering-agent-skill-
```

### Manual installation

Clone this repository into your agent's skills directory:

```bash
git clone https://github.com/mshanghai570/swiftui-engineering-agent-skill-.git swiftui-engineering
```

Common locations:
- **Manus (Cloud / Local):** `/home/ubuntu/skills/swiftui-engineering/` or `~/.manus/user-skills/swiftui-engineering/`
- **Claude Code:** `~/.claude/skills/swiftui-engineering/`

---

## Repository Structure

```
swiftui-engineering-agent-skill-/
├── SKILL.md        # The skill specification (frontmatter + instructions)
├── README.md       # This file
├── LICENSE         # MIT License
└── .gitignore
```

---

## License

[MIT](LICENSE) © mshanghai570
