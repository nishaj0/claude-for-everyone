# claude-for-everyone

Skills, plugins, MCP servers and rule files for Claude Code, Codex, Antigravity and other coding agents, organised by what you want to do. Each entry says what it is and links to its repo.

> Free or freemium only: no paid-only tools. Seed list built from one person's GitHub stars, a report on 38 Instagram Reels, and GitHub popularity rankings (checked 3 Nov 2026). I haven't checked every license or pricing page. Entries were categorised from descriptions, not from reading every README. Install steps are left out on purpose: follow each repo's README.

## Contents

- **[Video](#video)**: [Editing](#editing) · [Motion Graphics](#motion-graphics) · [Animation Styles](#animation-styles) · [Prompts](#prompts)
- **[Audio](#audio)**: [Sound Effects](#sound-effects)
- **[Design](#design)**: [UI](#ui) · [Diagrams](#diagrams) · [Logo & Brand](#logo--brand) · [Web Animation & 3D](#web-animation--3d)
- **[Marketing](#marketing)**: [SEO](#seo) · [Social Content](#social-content) · [Sales Outreach](#sales-outreach)
- **[Dev](#dev)**: [Workflow & Planning](#workflow--planning) · [Quality & Token Saving](#quality--token-saving) · [Memory & Context](#memory--context) · [Browser & Web Access](#browser--web-access) · [Docs Lookup](#docs-lookup)
- **[Games](#games)**: [Effects & Mods](#effects--mods)
- **[Career](#career)**: [Job Search](#job-search)
- **[Discovery](#discovery)**: [Skill & Plugin Directories](#skill--plugin-directories)
- **[Standalone](#standalone)**: [Media Tools](#media-tools) · [Local Models & OCR](#local-models--ocr) · [Apps, Agents & Examples](#apps-agents--examples)
- **[Playbooks](PLAYBOOKS.md)**: video stacks · general patterns
- **More**: [Planned](#planned-empty) · [Types](#types-used-in-tables) · [Security](#security) · [Contributing](#contributing)


## Video

### Editing

Let an agent cut, caption and assemble video from your footage.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [openfilm](https://github.com/openfilm/openfilm) | skill + desktop app | Turns an agent into a video editor: cuts filler words, picks shots, adds captions, B-roll and music, exports MP4 or CapCut drafts. | You want agent-edited video you can still tweak on a timeline. |
| [concat](https://github.com/jub0t/concat) | app + agent hookup | Free local CapCut replacement (auto-captions, background removal, 4K export, no watermark) that Claude Code can drive. | You want a normal editor that the agent can also operate. |

See also: [stacks](PLAYBOOKS.md) for the full toolchain, and [standalone media tools](#media-tools) for tools like WhisperX and yt-dlp.

### Motion Graphics

Code-driven video: the agent writes HTML, GSAP or Canvas and renders it to MP4.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [hyperframes](https://github.com/heygen-com/hyperframes) | framework + skills | Write HTML/CSS/GSAP, render frame-accurate MP4. Built for agents. | You want videos authored as code (motion graphics, overlays, explainers). |
| [huashu-motion](https://github.com/alchaincyf/huashu-motion) | skill | Open-source Claude Motion alternative: code-driven launch films with transitions, generated music and a browser editor. | You want a launch or product film without a Teams/Enterprise plan. |
| [brag](https://github.com/latent-spaces/brag) | skill | One command turns a codebase into a launch video plus a caption. | You want a quick demo or launch video of your project. |
| [super-video-maker-skill](https://github.com/Bomx/super-video-maker-skill) | skill | Example of the "interview, toolbox, proof" delegation playbook, applied to video making. | You want a worked example of a well-structured skill. |

### Animation Styles

Style skills for stylised animated films and shorts. Pick one per project.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | skill | 43-59 code-drawn film styles (watercolor, crayon, pixel game, woodblock...), with music and narration. | You want a stylised animated short. |
| [onetake](https://github.com/feitangyuan/onetake) | skill | Product launch films as one continuous camera move with no hard cuts. | You want a single-take product film. |
| [gbro-collage-broll](https://github.com/pyang5166/gbro-collage-broll) / [VOX-COLLAGE-BROLL](https://github.com/MegaTroll222/VOX-COLLAGE-BROLL) | skill | Turns spoken script lines into Vox-style halftone paper-cutout collage B-roll. | You want editorial B-roll for talking-head videos. |
| [ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | starter kit + skill | p5.js hand-painted 2D watercolor cartoons across 31 emotions. | You want painterly 2D character animation. |
| [claude-animated-shorts](https://github.com/mromidev/claude-animated-shorts) | skill | Animated story shorts (2D characters in a 3D world) with three.js + Remotion. | You want short animated stories. |
| [stickman-video-director](https://github.com/kaomei/stickman-video-director) | skill | Turns an article or idea into a 6-scene storyboard and six prompts for Gemini Omni Flash (about 60s). | You want a quick stickman explainer. |
| [hypit](https://github.com/hypit-ai/hypit) | skill | Used for digital-mascot shorts (see the faceless mascot stack). | You're building mascot-based shorts. |

### Prompts

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) | collection | 700+ prompts for motion graphics, explainers, 3D scenes and games. | You want prompt ideas to copy. |


[↑ Contents](#contents)

## Audio

### Sound Effects

Fix the weak point of agent-made video: its sound effects.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [Clipwing/skills (real-sfx)](https://github.com/Clipwing/skills) | skill | Places real recorded sound effects on the exact action frame of a render or HyperFrames timeline. Includes 78 CC0 UI sounds and keeps existing voice and music. | You want proper sound design on a video edit. |
| [earshot](https://github.com/Leonxlnx/earshot) | MCP server + CLI | Lets the agent "listen": audits sync (e.g. a hit 80 ms late), reads loudness and spectrograms, and generates sound effects in code. | You want the agent to check and fix audio timing. |
| [Openverse API](https://github.com/wordpress/openverse) | free API | 5M+ openly licensed sounds, no key needed. The agent can search and download CC0 effects. | You need free sound effects without signing up for anything. |

Used together: Openverse to find sounds, real-sfx to place them, earshot to review the result.


[↑ Contents](#contents)

## Design

### UI

Make agents produce better-looking interfaces.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [impeccable](https://github.com/pbakaus/impeccable) | skill | Design vocabulary for the agent (`polish`, `bolder`, `critique`, `audit`) and catches generic "AI slop" UI. | You want to steer or review a frontend's look and feel. |
| [awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | collection | `DESIGN.md` files extracted from well-known brands' design systems. | You want the agent to build UI in the style of a specific brand. |
| [awesome-design-skills](https://github.com/bergside/awesome-design-skills) | collection | 67 `DESIGN.md` / `SKILL.md` design skills for Claude Design, Stitch, Codex, Cursor. | You want ready-made design styles. |
| [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | skill | Generates a project design system from a catalogue of styles, colour palettes and font pairs. | You want a consistent design system for a new project. |
| [taste-skill](https://github.com/Leonxlnx/taste-skill) | skill | Art direction, real photos and browser checks so designed sites look less generic. | Your AI-built pages look bland and samey. |

### Diagrams

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [diagram-design](https://github.com/cathrynlavery/diagram-design) | skill | 45 diagram types as self-contained HTML + SVG, without Mermaid-style output. | You need architecture, flow or explainer diagrams. |
| [archify](https://github.com/tt-a1i/archify) | skill | Turns a description, plan or repo into an interactive, shareable HTML diagram. | You want a clickable architecture diagram of a codebase or plan. |

### Logo & Brand

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [logo-design-skill](https://github.com/kaankiziltug/logo-design-skill) | skill | Logo process (brief, concepts, SVG craft, testing) plus a library of 1,400+ reference logos. | You need a logo or brand mark. |

### Web Animation & 3D

Teach the agent to build award-style animated sites and interactive 3D.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [scroll-craft](https://github.com/nateherkai/scroll-craft) | plugin | Scroll-driven site animation (Next.js, GSAP, Three.js, Lenis style). | You want scroll-triggered, high-end landing pages. |
| [gsap-skills](https://github.com/greensock/gsap-skills) | plugin | Official GreenSock skills for GSAP and ScrollTrigger. | You want correct GSAP code from the agent. |
| [webgl-animation-skills](https://github.com/iart-ai/webgl-animation-skills) | skill | WebGL and Three.js animation skills. Sibling repos: `iart-ai/motion-skills`, `iart-ai/web-animation-skills`. | You're building WebGL hero sections or 3D scenes. |
| [anatomy](https://github.com/wheresryan22/anatomy) | skill | Interactive 3D anatomy-style exploded views of systems. | You want to explain how something is built, visually. |
| [machine-skill](https://github.com/AirsupHQ/machine-skill) | skill | `/machine a turbofan jet engine` renders an interactive 6-layer exploded WebGL model with live controls. | You want interactive 3D explainers of machines. |


[↑ Contents](#contents)

## Marketing

### SEO

No plugin or skill entries yet. Candidates to add: SEO audit, keyword research and content-brief skills.

The standalone [open-seo](#apps-agents--examples) (Semrush/Ahrefs alternative) is an app, not a plugin.

### Social Content

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill) | 13 skills | Reel writer with 26 hook formulas and hook scoring, plus a virality skill that ranks Reels in your niche and rewrites ideas in your voice. | You make Instagram Reels and want hooks and ideas. |
| carousel-studio ([guide](https://milleemd.com/guides/instagram-carousel-system/)) | skill (zip) | Writes and renders branded 1080x1350 Instagram carousels from a topic. 6 style presets, or use Canva's MCP. | You make carousels. |
| [reddit-automation](https://github.com/flowkit-labs/skills) | skill | Finds Reddit threads where people need help and drafts transparent replies. | You do community-led marketing. Post replies yourself and follow each subreddit's rules. |

### Sales Outreach

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [harvey](https://github.com/ethanplusai/harvey) | agent on Claude Code / Codex | Finds local businesses, reads their sites, writes cold emails that mention something real, handles replies. Per its demo nothing sends without your approval. | You want outbound sales automated. It emails real people, so review everything. |


[↑ Contents](#contents)

## Dev

### Workflow & Planning

Add structure to how the agent plans, reviews and tests, so it stops jumping straight into code.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [superpowers](https://github.com/obra/superpowers) | skills | Makes the agent brainstorm, write implementation plans, and verify its own work. | You want a disciplined plan-then-build loop. |
| [gstack](https://github.com/garrytan/gstack) | slash commands | Garry Tan's setup: 23 specialist commands (CEO review, eng manager, designer, QA in a real browser, release engineer that opens the PR). | You want role-based review at each stage. |
| [ponytail](https://github.com/DietrichGebert/ponytail) | plugin | Makes the agent ask whether code needs to exist before writing it. | The agent over-builds. |
| [vibe-wise](https://github.com/nykooi1/vibe-wise) | plugin (Claude Code + Codex) | Asks how *you* would build it and won't write code until you approve the design. | You want to understand what the agent builds, not just ship it. |
| [mattpocock/skills](https://github.com/mattpocock/skills) | skills | `grill-me` (stress-tests your plan), `grill-with-docs` (checks plans against your docs and ADRs), `improve-codebase-architecture` (finds coupling to fix). | You want a plan challenged before coding. |
| tdd ([nulfrog/skills](https://www.skills.sh/nulfrog/skills/tdd), [superpowers](https://www.skills.sh/obra/superpowers/test-driven-development)) | skill | Enforces a strict red-green-refactor loop. | You want test-first development. |
| [everything-claude-code (ECC)](https://github.com/affaan-m/ECC) | plugin | A bundle of skills, agents, hooks and rules for planning, testing and self-review. | You want one big ready-made setup instead of picking pieces. |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | skills | Engineering skills for each stage from spec to ship, behind nine slash commands. | You want a stage-by-stage build process. |
| [planning-with-files](https://github.com/OthmanAdi/planning-with-files) | plugin | Keeps plans in markdown files with checklists so work survives a context reset or crash. | Long tasks lose their plan when the context fills up. |

### Quality & Token Saving

Get better behavior from coding agents and spend fewer tokens or dollars.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | CLAUDE.md | One `CLAUDE.md` that counters common LLM coding mistakes, based on Karpathy's observations. | You want a drop-in rule file for more careful coding. |
| [caveman](https://github.com/JuliusBrussee/caveman) | skill + proxy | Makes the agent answer in terse "caveman" style, cutting output tokens by about 65%. | Your sessions are long or you're hitting usage limits. |
| [TokenEconomizer](https://github.com/microsoft/TokenEconomizer) | tool | Black-box cost control for coding agents, based on past experience. | You want to cut spend without changing prompts by hand. |
| [9router](https://github.com/decolua/9router) | router | Connects Claude Code, Codex, Cursor, Cline and Copilot to 40+ providers with auto-fallback and token trimming. | You keep hitting rate limits or want cheaper or free models as fallback. |
| [codegraph](https://github.com/colbymchenry/codegraph) | MCP / index | Pre-indexed code knowledge graph that syncs on change. Fewer tool calls and tokens for code exploration. | You work in a large codebase and the agent wastes tokens searching. |
| [gemini-mcp-tool](https://github.com/jamubc/gemini-mcp-tool) | MCP | Lets the agent call Gemini CLI to use its huge context window. | You need to analyse files too large for the main model's context. |
| [CodeBurn](https://codeburn.app) | tool | Tracks token usage and cost locally across about 40 tools. Free and open source per the roundup I read. | You want to see where your tokens and money go. |

Cost tips from the source report are in [../general/playbooks.md](PLAYBOOKS.md).

### Memory & Context

Stop the agent forgetting everything between sessions.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [engram](https://github.com/Gentleman-Programming/engram) | MCP server + CLI | Persistent memory for coding agents (Go, SQLite + FTS5, with MCP, HTTP API and TUI). Works with any agent. | You want decisions and fixes remembered across sessions and tools. |
| [claude-mem](https://github.com/thedotmack/claude-mem) | plugin | Automatically saves what you worked on and injects relevant context next session. | You want memory with no manual saving. |
| [base](https://github.com/ChristopherKahler/base) | workspace system | "Builder's Automated State Engine": a Claude Code workspace that remembers and maintains itself. | You want a structured, self-maintaining project workspace. |
| [codegraph](https://github.com/colbymchenry/codegraph) | MCP / index | Code knowledge graph that stays in sync with your code. | The agent needs to understand a big codebase's structure quickly. |
| [obsidian-skills](https://github.com/kepano/obsidian-skills) | skills | By Obsidian's CEO: teaches the agent to read and write Obsidian Markdown, Bases and JSON Canvas. | Your notes live in Obsidian and you want the agent to use them. |
| [Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) | plugin | Builds a knowledge graph of a codebase with a dashboard to explore it. | You're new to a codebase and want a map of it. |

### Browser & Web Access

Let the agent read, search, browse and scrape the web.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [Agent-Reach](https://github.com/Panniantong/Agent-Reach) | skill + CLI | Free read/search of 13+ platforms (YouTube transcripts, X, Reddit, GitHub, Instagram, TikTok, LinkedIn, RSS, Bilibili, Xiaohongshu, web pages). | You need content from social platforms that normal web fetch can't get. |
| [playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Microsoft's Playwright browser automation server. | You want the agent to click through sites, test UIs or fill forms. |
| [agent-browser](https://github.com/vercel-labs/agent-browser) | skill + CLI | Headless browser CLI for agents to navigate, click, fill forms and screenshot. | You want a lighter browser tool than a full MCP. |
| [obscura](https://github.com/h4ckf0r0day/obscura) | tool | Headless browser built for AI agents and scraping (Rust). | You need fast, lightweight scraping. |

### Docs Lookup

Give the agent current library documentation instead of stale training data.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [context7](https://github.com/upstash/context7) | MCP server + plugin | Pulls version-specific library docs into the agent's context so generated code matches the versions you use. Free to use; an API key is optional (per the roundup I read, not checked on the vendor site). | The agent keeps writing outdated API calls. |


[↑ Contents](#contents)

## Games

### Effects & Mods

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [pixelfx](https://github.com/patch-gg/pixelfx) | library + skill | 200+ pixel-art game effects (spells, explosions, weather, slash hits) drawn from code, MIT licensed. | You're making a pixel-art game and need VFX sprites. |
| [coop-anything](https://github.com/cranebeaker/coop-anything) | agent playbook | Name a game you own and the agent finds, fixes or builds a co-op mod (friends join via Steam). | You want to play a single-player game in co-op. |

> Needs more entries: Godot, Unity, Unreal, Phaser and Three.js skills.


[↑ Contents](#contents)

## Career

### Job Search

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [ai-job-search](https://github.com/ai-job-search-dev/ai-job-search) | framework on Claude Code | Evaluates job postings, tailors your CV, writes cover letters and preps interviews. Fork it and run it locally. | You're job hunting and want it automated. |


[↑ Contents](#contents)

## Discovery

### Skill & Plugin Directories

Where to find more.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [skills.sh](https://www.skills.sh/) | directory | Leaderboard of agent skills ranked by real install count. | You want to see what's popular. |
| [vercel-labs/skills](https://github.com/vercel-labs/skills) | CLI + `find-skills` skill | The open agent-skills installer (`npx skills`). `find-skills` lets the agent search and install skills mid-session. | You want to install skills from the command line, or let the agent find them. |
| [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) | list | Curated list of Claude Skills, resources and tools. | You want to browse what exists. |
| [awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) | list | Curated list of Claude video skills. | You want more video skills than are in this repo. |
| [awesome-design-skills](https://github.com/bergside/awesome-design-skills) | list | 67 design skill files. | See [design/ui](#ui). |
| [wshobson/agents](https://github.com/wshobson/agents) | plugin marketplace | Marketplace of about 94 plugins that works across Claude Code, Codex, Cursor, OpenCode, GitHub Copilot, Google Antigravity and Pi. | You want plugins that work in more than one agent. |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | collection | About 380 skills, agents and commands across engineering, marketing, product, compliance, research and finance, for Claude Code, Codex, Gemini CLI, Cursor and others. | You want a wide pool of skills outside coding, such as marketing and finance. |
| [top-claude-code-skills](https://github.com/selan-ai/top-claude-code-skills) | ranking | Claude Code skills ranked daily from GitHub: all time, this week, this month. | You want to see what's popular right now. |
| [awesome-claude-code-skills](https://github.com/itgoyo/awesome-claude-code-skills) | list | Curated list of top-starred Claude Code tools and skills. | You want to browse more. |

**Security:** skills run commands on your machine. One reel in the source report cites a study that found 1 in 4 of 31,000+ skills had a security flaw. That claim is unverified, but read a skill before installing it.


[↑ Contents](#contents)

## Standalone

### Media Tools

Apps, models and datasets for video, image, audio and 3D. They run on their own and don't plug into Claude, Codex or Antigravity (though an agent can call the CLI ones from a shell).

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [AI-Youtube-Shorts-Generator](https://github.com/Anil-matcha/AI-Youtube-Shorts-Generator) | app | Open-source Opus Clip alternative: LLM picks highlights, Whisper transcribes, auto-crops to 9:16. | You want to turn long YouTube videos into vertical shorts. |
| [hotclip](https://github.com/xixihhhh/hotclip) | app | Local AI clipper for long videos, livestream replays and podcasts. Adds subtitles and converts to vertical, with publishing aimed at Chinese platforms. | You work with livestreams or publish to Douyin, Bilibili or Xiaohongshu. |
| [upscayl](https://github.com/upscayl/upscayl) | desktop app | Free AI image upscaler for Linux, macOS and Windows. | You need to enlarge or sharpen images. |
| [MisoTTS](https://github.com/MisoLabsAI/MisoTTS) | model | 8B-parameter expressive text-to-speech model. | You want AI voiceovers. |
| [VoiceStudio](https://github.com/debpalash/voicestudio) | app | Local, CPU-only voice cloning and dubbing in 646 languages from 5-15 seconds of audio; offline speech-to-text. An ElevenLabs alternative. | You want private voice cloning without cloud APIs. |
| [fish-speech](https://github.com/fishaudio/fish-speech) | model | Voice cloning (Fish Audio's open model). | You want to clone a voice for voiceovers. |
| [Rhubarb Lip Sync](https://github.com/DanielSWolf/rhubarb-lip-sync) | CLI | Maps the phonemes in an audio track to mouth shapes (A-H) for 2D characters. | You're animating a talking mascot. |
| [WhisperX](https://github.com/m-bain/whisperx) | CLI | Local speech-to-text with word-level timestamps. | You need transcripts or silence/jump-cut detection. |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | CLI | Downloads reference videos and audio. | You need source clips. |
| [NVIDIA SimReady Central](https://huggingface.co/spaces/nvidia/simready-central) | dataset | 2,600+ physics-ready OpenUSD 3D models, CC BY 4.0, for Isaac Sim, PhysX, Newton and MuJoCo. | You're doing robotics or physics simulation. |

CLI tools such as WhisperX, yt-dlp and Rhubarb show up in the [video stacks](PLAYBOOKS.md).

### Local Models & OCR

Run models on your own hardware, or read documents with AI. Not agent plugins.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [airllm](https://github.com/lyogavin/airllm) | library | Runs very large LLMs on a single 4GB GPU. | You have a weak GPU and want to try big models. |
| [colibri](https://github.com/JustVugg/colibri) | inference engine | Runs large mixture-of-experts models by spreading experts across GPU, RAM and NVMe (C). | You want a frontier-size MoE model on consumer hardware. |
| [FreeToken](https://github.com/FlashML-org/FreeToken) | serving | Runs massive models fast on a desktop. | You want local serving instead of paid API calls. |
| [Unlimited-OCR](https://github.com/baidu/Unlimited-OCR) | model | Baidu's OCR for long, one-shot document parsing. | You need to extract text from long PDFs or scans. |

### Apps, Agents & Examples

Full products, separate agents and demo projects. Useful, but you run them instead of installing them into Claude, Codex or Antigravity.

| Name | Type | What it does | Use it when |
|---|---|---|---|
| [open-codesign](https://github.com/OpenCoworkAI/open-codesign) | app | Open-source Claude Design alternative: prompt to prototype, slides or PDF. Multi-model, bring your own key. | You want a design tool that isn't tied to one vendor. |
| [open-seo](https://github.com/every-app/open-seo) | app | Open-source alternative to Semrush and Ahrefs. | You want keyword and SEO data without paid tools. |
| [jcode](https://github.com/1jehuang/jcode) | agent harness | Rust terminal coding agent that replaces Claude Code's harness. Boots in about 14 ms, auto-memory, multi-agent on one repo. The "20x more efficient" figure is the reel's claim. | You want a different, lighter coding agent instead of adding to Claude Code. |
| [BettaFish](https://github.com/666ghj/BettaFish) | multi-agent app | Public-opinion analysis: collects and analyses online discussion and predicts trends. | You're doing sentiment or trend research. |
| [hermes-agent](https://github.com/NousResearch/hermes-agent) | agent | Nous Research's own agent that "grows with you". | You want a separate agent to use instead of Claude Code. |
| [paperclip](https://github.com/paperclipai/paperclip) | app | Manages a team of agents at work. | You're running several agents and need one place to manage them. |
| [OpenMausBot](https://github.com/milind-soni/OpenMausBot) | bot | Open-source Grok Bot alternative with a VM the bots can use. | You want a bot that runs tasks on its own machine. |
| [Claude-of-Duty](https://github.com/mshumer/Claude-of-Duty) | example | A Call of Duty-style FPS in Three.js, built from a single prompt. | You want to see what a one-prompt 3D game looks like. |


[↑ Contents](#contents)

## Playbooks
Multi-tool recipes (video editing stacks, sound-effects pipeline, mascot shorts) and general patterns (delegation, shared second brain, saving credits) are in [PLAYBOOKS.md](PLAYBOOKS.md).


[↑ Contents](#contents)

## Planned (empty)
Writing, data & analytics, testing & QA, DevOps, security, documentation, finance, education, and more SEO entries.


[↑ Contents](#contents)

## Types used in tables
`skill` · `plugin` · `MCP` (server the agent calls) · `CLAUDE.md` (rules file) · `collection` / `list` · `app` · `model`


[↑ Contents](#contents)

## Security
Skills and plugins run commands on your machine. Read one before you add it, and take extra care with anything that sends email, posts online or spends money.


[↑ Contents](#contents)

## Contributing
Add a row to the right section above. See [CONTRIBUTING.md](CONTRIBUTING.md).
