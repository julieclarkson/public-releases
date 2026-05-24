# Julie J. Clarkson — AI IDE Plugins

Free, local-only plugins that turn your AI coding tool into a full content pipeline. Capture what you build, generate case studies, record video demos, launch on GitHub, and publish blog posts — all from inside your editor.

No SaaS. No accounts. No cloud uploads. Everything runs locally in your project folder.

Works in **Claude, Cursor, Codex, VS Code, Cowork**, and any AI tool with chat.

---

## How to install any plugin

Every plugin follows the same 4-step process:

1. **Download** — Go to the [Releases](https://github.com/julieclarkson/public-releases/releases) page and download the `.zip` for the plugin you want
2. **Extract** — Unzip the file. You'll get a folder that starts with a dot (e.g., `.case-study-maker-plugin`)
3. **Drag** — Move the folder into your project directory
4. **Start** — Open your project in your AI tool and say: **"start [plugin-name]"**

The plugin auto-detects your editor and sets everything up. No configuration needed.

---

## The plugins

### Case Study Maker

Capture build decisions as you code. Generate portfolio and marketing case studies from the real decisions you made — not from memory weeks later. Includes **Writing Rubric** for voice calibration, so every output across all plugins sounds like you.

**Say:** "start case-study-maker"

---

### Demo Maker

Auto-generate narrated MP4 product demos from your codebase. Point it at your project, review the script, hit render. You get 6 platform-ready videos — Full, GitHub, Twitter, Product Hunt, Instagram, and TikTok — each with correct dimensions, timing, and narration.

**Say:** "start demo-maker"
**Optional:** Add an ElevenLabs API key for voice narration. Without one, demos work in caption-only mode.
**Requires:** Node.js 18+, FFmpeg

---

### Git Launcher

Generate launch-ready GitHub assets from your codebase — automatically. Get a polished README, desktop/tablet/mobile screenshots, Mermaid architecture diagrams, a 1200x630 social preview image, and platform-specific launch posts for Reddit, Hacker News, Twitter/X, Product Hunt, and Dev.to.

**Say:** "start git-launcher"
**Requires:** Node.js 18+

---

### Post Maker

Turn your build artifacts into publication-ready blog posts. Post Maker reads your case studies, demos, and code, then interviews you, drafts in your voice, validates every claim, and formats output for Substack, LinkedIn, Dev.to, Medium, Hashnode, newsletters, Twitter/X, and Bluesky.

**Say:** "start post-maker"
**Requires:** Node.js 18+, Case Study Maker active in the same project

---

### Writing Rubric

Teach any AI tool what makes writing yours — and let it be an honest editor. Three interviews build a voice profile and a weighted quality rubric. After that, any AI tool can evaluate any piece of writing against your personal standards.

**Bundled with Case Study Maker.** Also available as a standalone download.
**Say:** "start writing-rubric"

---

## Recommended install order

1. **Case Study Maker** first — sets up voice calibration and reflection capture
2. Then any combination of **Demo Maker**, **Git Launcher**, and **Post Maker**

Each plugin reads the previous plugin's output to enrich its own. Case Study Maker's reflections feed into demo scripts, launch posts, and blog articles.

---

## What you need

- **Any AI tool with chat** — Claude, Cursor, Codex, VS Code with AI, Cowork, or anything that reads project files
- **Node.js 18+** — required for Demo Maker, Git Launcher, and Post Maker. Optional for Case Study Maker and Writing Rubric.
- **No API keys** — all plugins work without API keys. Demo Maker optionally uses ElevenLabs for voice narration.

---

## Security

All plugins are local-only. No data leaves your machine. No network calls, no cloud uploads, no telemetry. API keys (when used) load from `.env` files inside the plugin workspace — never from chat. Init scripts use safe argument passing to prevent injection. Generated HTML includes Content-Security-Policy headers. Full security details are included in each plugin's `SECURITY_LOG.md`.

---

## License

All plugins are released under the **MIT License**. Free to use, modify, and distribute.

Published by **Julie J. Clarkson** / **Jacobus Company, LLC**, United States.

- [Terms of Service](https://julieclarkson.com/terms.html)
- [Privacy Policy](https://julieclarkson.com/privacy.html)
- [Liability Waiver](https://julieclarkson.com/liability.html)
