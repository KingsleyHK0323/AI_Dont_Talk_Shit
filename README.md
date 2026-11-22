<div align="center">

  <h1>⚡ AI Don't Talk Shit</h1>

  <p>
    <b>Enforce strict, zero-fluff, conclusion-first communication across AI models and agent platforms.</b>
  </p>

  <p>
    <img src="https://img.shields.io/github/license/KingsleyHK0323/AI_Dont_Talk_Shit?style=for-the-badge" alt="License: MIT" />
    <img src="https://img.shields.io/badge/Format-SKILL.md-blue?style=for-the-badge" alt="Format: SKILL.md" />
    <img src="https://img.shields.io/badge/Version-1.2.0-green?style=for-the-badge" alt="Version: 1.2.0" />
    <img src="https://img.shields.io/badge/Mode-Zero--Fluff-black?style=for-the-badge" alt="Mode: Zero-Fluff" />
  </p>

  <p>
    <a href="#overview">Overview</a> •
    <a href="#key-features">Key Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#behavioral-rules">Rules</a> •
    <a href="#repository-structure">Structure</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#license">License</a>
  </p>

</div>

<hr />

## Overview

**AI Don't Talk Shit** is a platform-agnostic `SKILL.md` directive designed to eliminate conversational overhead, enforce immediate conclusion delivery, and maximize signal-to-noise ratio in AI responses. It strips away preambles, platitudes, and closing pleasantries while keeping technical outputs accurate, structured, and actionable.

> [!IMPORTANT]
> **Core Principle:** Deliver the direct answer in the first sentence, eliminate filler and sign-offs, and never sacrifice factual accuracy for brevity.

<hr />

## Key Features

<table>
  <tr>
    <td width="50%">
      <h3>🎯 Conclusion First</h3>
      <p>Requires the opening sentence to state the direct answer, primary solution, or core output with zero introductory buildup.</p>
    </td>
    <td width="50%">
      <h3>🚫 Zero Fluff & Platitudes</h3>
      <p>Eliminates conversational filler (<em>"Sure, I can help with that"</em>), AI clichés, and trailing pleasantries (<em>"Hope this helps!"</em>).</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>⚡ High Signal Density</h3>
      <p>Prioritizes structured lists, tables, and language-tagged code blocks over verbose paragraphs and redundant summaries.</p>
    </td>
    <td width="50%">
      <h3>🌐 Cross-Platform Ready</h3>
      <p>Works as a <code>SKILL.md</code> skill or as a system prompt / custom instruction block across AI assistants and agent runtimes.</p>
    </td>
  </tr>
</table>

<hr />

## Installation

This repository distributes a standalone skill named `ai-dont-talk-shit`. Clone the repository first:

```bash
git clone [https://github.com/KingsleyHK0323/AI_Dont_Talk_Shit.git](https://github.com/KingsleyHK0323/AI_Dont_Talk_Shit.git)
cd AI_Dont_Talk_Shit
```

Install `SKILL.md` into your AI assistant environment:

<details>
<summary><b>Claude Code (CLI)</b></summary>

Copy `SKILL.md` into your global or project-level skills directory:

```bash
# Global installation
mkdir -p ~/.claude/skills/ai-dont-talk-shit
cp SKILL.md ~/.claude/skills/ai-dont-talk-shit/SKILL.md

# Or project-scoped installation
mkdir -p .claude/skills/ai-dont-talk-shit
cp SKILL.md .claude/skills/ai-dont-talk-shit/SKILL.md
```

</details>

<details>
<summary><b>Claude (Web & Desktop Apps)</b></summary>

Package the `ai-dont-talk-shit` folder containing `SKILL.md` into a `.zip` archive and upload it via **Settings → Capabilities / Skills** (check Anthropic's documentation for current UI labels).

</details>

<details>
<summary><b>Cursor, Gemini, ChatGPT, and Custom Agents</b></summary>

For environments that do not load `SKILL.md` natively, paste the Markdown body of `SKILL.md` (everything below the closing `---` frontmatter line) into your custom instructions, rules file, or system prompt.

</details>

<hr />

## Usage

Activate the skill in your assistant and ask direct questions or give operational tasks:

```text
How do I undo the last local git commit while keeping changes staged?
```

Expected response style:

```text
Run `git reset --soft HEAD~1`. This moves `HEAD` back one commit and leaves all changes in the index for recommitting.
```

<hr />

## Behavioral Rules

| Category | Enforced Standard |
|---|---|
| **Opening Line** | Direct answer or primary output in sentence one; zero preamble. |
| **Banned Filler** | No *"Sure, I can help..."*, *"Great question"*, or *"Here is what you asked for"*. |
| **Banned Closings** | No *"Hope this helps!"*, *"Let me know if..."*, or trailing recaps. |
| **Formatting** | Concise bullets, tables, and fenced code blocks with language tags. |
| **Accuracy** | No fabricated commands, metrics, or claims; use `<PLACEHOLDER>` when unknown. |

See [`SKILL.md`](SKILL.md) for the complete protocol and pre-delivery checklist.

<hr />

## Repository Structure

```text
.
├── SKILL.md      # Standard AI skill specification (frontmatter, behavioral rules, protocol, checklist)
├── README.md     # Repository overview, installation guide, and usage examples
└── LICENSE       # MIT License
```

<hr />

## Contributing

Contributions are welcome, particularly refinements that improve conciseness without losing technical accuracy.

1. Fork the repository and create a branch (`git checkout -b feat/tighten-rules`).
2. Update `SKILL.md` (and `README.md` if behavior or setup changes), keeping YAML frontmatter (`name` and `description`) valid.
3. Verify that examples and rules remain concise, accurate, and free of filler.
4. Open a pull request describing the change.

<hr />

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 Kingsley ([@KingsleyHK0323](https://github.com/KingsleyHK0323)).