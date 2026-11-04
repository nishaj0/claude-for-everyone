# Playbooks

Recipes and patterns, not installable plugins. Summarised from reels in a third-party report, so check each step against the repos. Back to the [list](README.md).


## Video editing stacks

Combinations of tools that work together. Each links to the entry that explains it. Taken from reels in a third-party report, so check each step against the repos.

### 1. Edit your own footage with Claude (the "AI video editor workspace")
Goal: cut, caption and add motion graphics to recorded video.

1. Make a folder (e.g. `AI Video Editor`) and open it in Cursor or VS Code with Claude Code or Codex.
2. Have the agent create four subfolders: `Raw/` (camera clips), `Projects/` (timelines, scripts, exports), `Signature Style/` (fonts, colours, reference videos, templates), `Setup/` (tool configs, agent rules, prompts).
3. Set up the toolchain: FFmpeg/ffprobe (cutting, audio, MP4 encoding), Python, Node.js, [HyperFrames](README.md#motion-graphics) (motion-graphic overlays), [WhisperX](README.md#media-tools) (transcripts and silence detection), [yt-dlp](README.md#media-tools) (reference clips), Playwright (frame capture).
4. Alternatively use [openfilm or concat](README.md#editing), which wrap much of this.

### 2. Add professional sound effects
Goal: replace the agent's weak default SFX. See [audio/sound-effects](README.md#sound-effects).

Openverse (find free sounds) + real-sfx (place at the exact frame) + earshot (listen back and fix off-sync or missing effects).

### 3. Faceless mascot shorts
Goal: a full short with no camera.

1. Add the `hypit` and `hyperframes` skills.
2. Make or record a voice track (VoiceStudio or fish-speech for cloning, see [standalone](README.md#media-tools)).
3. Draw mouth sprites A-H for your mascot and run Rhubarb Lip Sync to map each phoneme to a sprite.
4. Give the agent the sprites, audio and B-roll, and have it render through HyperFrames.

### 4. Stylised animated video ("Five Worlds")
Pick one style skill per project: HyperFrames (HTML motion graphics), onetake (single-camera product film), gbro-collage-broll (Vox-style collage), ClaudeAnimationBase (watercolor cartoons), lemo-opuscar (43-59 styles). See [motion-graphics](README.md#motion-graphics) and [animation-styles](README.md#animation-styles).

### 5. Launch video for a software project
[brag](README.md#motion-graphics): run `/brag` inside the project. Or [huashu-motion](README.md#motion-graphics) for a hand-directed launch film with a browser editor.

### 6. Modular creative studio (pattern, not a repo)
One reel shows nine separate `SKILL.md` folders (product-ad, paper-cut, content, animation, director, ad, studio, visual, creative-ad), chained in one window: director storyboards, visual skills generate imagery, animation skills add motion, ad skills write copy. The reel doesn't link a repo, so this is a structure to copy, not something you can install.


## General patterns

Guides and patterns, not installable plugins. Summarised from reels in a third-party report, so treat the numbers as the reels' claims.

### Run one agent with playbooks (the delegation pattern)
Instead of many small agents, run one and give it a playbook per job:
1. **Interview:** have the agent quiz you on inputs, edge cases, tone and failure modes, then write the answers into a `SKILL.md`.
2. **Toolbox:** save every working script and template in a `tools/` folder and link them in the playbook so it never rewrites the same helper.
3. **Proof:** put a definition-of-done checklist in the playbook. When it makes a mistake, fix the playbook rule rather than arguing in chat.

Worked example: [super-video-maker-skill](https://github.com/Bomx/super-video-maker-skill).

### Shared "second brain" across agents (Notion)
One Notion "Vault" connected to every agent through MCP, with five pages: **Soul** (rules and safety limits), **Memory** (facts, tagged by which agent wrote them), **Artifacts** (outputs), **Skills** (reusable instructions), **Lessons** (daily log of mistakes and corrections). Based on Notion co-founder Akshay Kothari's setup.

### Three weekend builds
Local second brain (Claude Code + Ollama + an Obsidian vault); a single-job inbox triage agent ("one agent, one job"); a localhost life dashboard (Vite, Tailwind, Supabase, Stripe).

### Save credits
- Match model and effort to the task: Sonnet for daily work, the biggest model only for deep multi-file refactors.
- The prompt cache expires (reel claims 1 hour on subscription plans, 5 minutes on API), so an idle session pays to rebuild its context. Finish or clear before breaks and leave a short handoff markdown file.
- The reel also mentions free cloud-session credits for Pro/Max plans. Check Anthropic's current terms, since that is unverified.

### Pre-launch checklist for AI-built apps (35 points, partial)
Privacy policy and terms linked in the footer and sign-up; working one-click unsubscribe; scheduled data-retention cleanup; remove fake countdown timers and other dark patterns; keyboard navigation, focus order, Escape to close and ARIA labels. The reel shows 35 items, but only these were captured.

### Context
- Cloud-agent pricing (one reel): Claude Duet is bundled in the $20 Pro plan, OpenAI's Dots come with ChatGPT Pro ($100-500/month), and Meta's Muse is free with a merchant transaction fee. The reel's claims, unchecked.
- Strategy (one reel): with 560K+ App Store launches in H1 2026, distribution and community matter more than building. The reel's claim, unchecked.
