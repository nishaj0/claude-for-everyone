# claude-for-everyone

A community-maintained list of skills, plugins, MCP servers and rule files for Claude, organised by what you want to do. Each entry says what it is and links to its repo.

> Free or freemium only: no paid-only tools. Contributions are welcome, see [CONTRIBUTING.md](CONTRIBUTING.md). Install steps are left out on purpose: follow each repo's README.
>
> **Caution:** entries are not security-audited. Review any skill, plugin or MCP server before installing it, see [Security](#security).

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
- **More**: [Planned](#planned-empty) · [Types](#types-used-in-tables) · [Security](#security) · [Contributing](#contributing)


## Video

### Editing

Let an agent cut, caption and assemble video from your footage.

| Name | Type | What it does |
|---|---|---|
| [openfilm](https://github.com/openfilm/openfilm) | skill + desktop app | Open-source AI video agent: Claude writes a film as HTML pages with a frame(t) function, and a local browser Studio editor lets you edit and render it (MIT; desktop app available). |
| [concat](https://github.com/jub0t/concat) | app + MCP server | Free, open-source, local video editor (CapCut alternative) with auto-captions, background removal, 4K export, no watermark, and a built-in MCP server (`concat --mcp`) for AI agents. |
| [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | skill | An Apache-2.0 Claude Code skill that builds cinematic product promo videos with Remotion from your own screenshots and copy. Remotion may need a paid license for companies. |
| [OpenMontage](https://github.com/calesthio/OpenMontage) | app | An AGPL-3.0 open-source agentic video production system with 12 pipelines and 100+ tools that turns Claude Code into a video studio. Optional paid API keys; AGPL-3.0. |
| [ffmpeg-skill](https://github.com/kajisho5/ffmpeg-skill) | MCP | A free MIT-licensed local video editor for coding agents with 42 FFmpeg tools and an MCP server that works with Claude Code. |

### Motion Graphics

Code-driven video: the agent writes HTML, GSAP or Canvas and renders it to MP4.

| Name | Type | What it does |
|---|---|---|
| [hyperframes](https://github.com/heygen-com/hyperframes) | framework + plugin | Open-source framework that turns HTML, CSS, media and seekable animations into deterministic MP4 videos, with a Claude Code plugin and skills for agents. |
| [huashu-motion](https://github.com/alchaincyf/huashu-motion) | skill | Skill that makes product launch films from a prompt: the agent writes the animation, composes the score, and opens a browser editor where you click on the picture to request changes (MIT). |
| [brag](https://github.com/latent-spaces/brag) | skill | Agent skill (/brag, plus a lean /brag-slim) that turns your project into a short launch video with music, motion and share copy; installs as a Claude Code plugin. |
| [super-video-maker-skill](https://github.com/Bomx/super-video-maker-skill) | skill | End-to-end video production skill: turns an idea, link, screen recording or script into a finished video using HeyGen avatars, AI b-roll, Remotion, HyperFrames, FFmpeg and captions. |

### Animation Styles

Style skills for stylised animated films and shorts. Pick one per project.

| Name | Type | What it does |
|---|---|---|
| [lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | skill | Toolbox of 66 film styles made in code (watercolor, crayon, pixel and more), each with its own short film; tuned for Claude Opus 5.5. |
| [onetake](https://github.com/feitangyuan/onetake) | skill | Claude skill for product launch films, teasers and demos made as one continuous camera take, where each beat grows out of the previous one with no hard cuts. |
| [gbro-collage-broll](https://github.com/pyang5166/gbro-collage-broll) / [VOX-COLLAGE-BROLL](https://github.com/MegaTroll222/VOX-COLLAGE-BROLL) | skill | Skill that turns a ~5s spoken script line into a halftone paper-cutout collage B-roll clip via a three-gate approval flow; the VOX version is a Claude Code skill, gbro needs separate image-generation tools. |
| [ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | starter kit | Starter kit for animating a character (Clawd) in p5.js and p5.brush with Claude Opus 5.5, with an animation guide and render scripts for hand-painted watercolor-style 2D video. |
| [claude-animated-shorts](https://github.com/mromidev/claude-animated-shorts) | skill | Free Claude skill for 55-70 s vertical animated story shorts: 2D characters in a 3D world, rendered with three.js in Remotion locally with synthesized sound. |
| [stickman-video-director](https://github.com/kaomei/stickman-video-director) | skill | Skill that turns a topic, article or script into animated stickman videos for faceless YouTube channels, with 10 visual styles, in a storyboard-and-prompts Director mode or an Autopilot mode. |
| [hypit](https://github.com/hypit-ai/hypit) | skill | Open-source skill and runtime that lets Claude clone or create videos (footage, captions, B-roll, effects anchored to words) from a text-based video workflow format. |

### Prompts

| Name | Type | What it does |
|---|---|---|
| [awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) | collection | Collection of 703 prompts from viral videos made with Claude Opus 5.5 (motion graphics, explainers, 3D scenes, games), each with the creator's prompt or original post. |


[↑ Contents](#contents)

## Audio

### Sound Effects

Fix the weak point of agent-made video: its sound effects.

| Name | Type | What it does |
|---|---|---|
| [Clipwing/skills (real-sfx)](https://github.com/Clipwing/skills) | collection | Collection of agent skills from Clipwing, including Real SFX (places real recorded sound effects on the exact frame, ships 78 CC0 UI sounds) and HyperFrames to After Effects. |
| [earshot](https://github.com/Leonxlnx/earshot) | MCP server + CLI | Gives Claude ears: describes and measures audio, audits sync and loudness, finds the best moment, and generates sound effects in code; runs locally as a CLI, Python API and MCP server. |
| [Openverse API](https://github.com/wordpress/openverse) | API | Openverse, WordPress's search engine and API for openly licensed media including audio; the repo is the search engine's source, not an agent skill. |

Used together: Openverse to find sounds, real-sfx to place them, earshot to review the result.


[↑ Contents](#contents)

## Design

### UI

Make agents produce better-looking interfaces.

| Name | Type | What it does |
|---|---|---|
| [impeccable](https://github.com/pbakaus/impeccable) | skill | Design skill that gives the agent a design vocabulary (polish, bolder, critique, audit) to steer UI work and catch generic AI-looking design. |
| [awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | collection | Curated collection of ready-to-use DESIGN.md files extracted from real websites' design systems, which an agent reads to generate visually consistent UI. |
| [awesome-design-skills](https://github.com/bergside/awesome-design-skills) | list | Curated registry of 67 design-system skill files (each with SKILL.md and DESIGN.md) that you pull into a project with `npx typeui.sh pull`. |
| [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | skill | Skill that generates a tailored project design system from searchable databases of UI styles, colour palettes and font pairings, using a reasoning engine over 192 rules. |
| [taste-skill](https://github.com/Leonxlnx/taste-skill) | skill | Skill that gives the agent an art direction, real credited photos and a real-browser check so the websites and app screens it builds look less generic. |
| [magic-mcp](https://github.com/21st-dev/magic-mcp) | MCP | Searches React/Tailwind components and generates UI from your editor. Needs a free API key. |
| [frontend-slides](https://github.com/zarazhangrui/frontend-slides) | plugin | A free Claude Code plugin that generates single-file HTML presentations from scratch or from PowerPoint files. |
| [garden-skills](https://github.com/ConardLi/garden-skills) | skill | A free MIT-licensed collection of skills for web design, image generation, video and knowledge-base retrieval, tested with Claude Code and Claude.ai. |
| [hallmark](https://github.com/Nutlope/hallmark) | skill | A free MIT-licensed design skill from Together AI that helps Claude Code build web pages that do not look AI-generated. |
| [skills](https://github.com/jakubkrehel/skills) | skill | A free MIT-licensed collection of skills for reviewing and building interfaces, covering accessibility, layout, typography, color and writing, installable as a Claude Code plugin. |

### Diagrams

| Name | Type | What it does |
|---|---|---|
| [diagram-design](https://github.com/cathrynlavery/diagram-design) | skill | Skill that draws diagrams as one self-contained HTML + SVG file in your brand, with 45 diagram types and no Mermaid-style output. |
| [archify](https://github.com/tt-a1i/archify) | skill | Turns an idea, question, plan or repo description into an interactive HTML page you can explore, customize and share, from itineraries to system diagrams. |

### Logo & Brand

| Name | Type | What it does |
|---|---|---|
| [logo-design-skill](https://github.com/kaankiziltug/logo-design-skill) | skill | Logo-design skill covering brief, concepts, SVG construction and testing, with a searchable library of 1,400+ real SVG logos and Python tools for auditing and exporting. |
| [dashboard-icons](https://github.com/homarr-labs/dashboard-icons) | MCP | 3,400+ curated dashboard icons and logos, with a free MCP server. |

### Web Animation & 3D

Teach the agent to build award-style animated sites and interactive 3D.

| Name | Type | What it does |
|---|---|---|
| [scroll-craft](https://github.com/nateherkai/scroll-craft) | plugin | Skill, also packaged as a Claude Code plugin, for building premium scroll-driven websites with a design workflow, engine and verification tools. |
| [gsap-skills](https://github.com/greensock/gsap-skills) | plugin | Official GreenSock agent skills that teach correct GSAP usage: core API, timelines, ScrollTrigger, plugins, framework integrations and performance. |
| [webgl-animation-skills](https://github.com/iart-ai/webgl-animation-skills) | skill | Skills for WebGL animation: GLSL fragment shaders, Three.js scene animation, and particle systems; installable as a Claude Code plugin marketplace. |
| [anatomy](https://github.com/wheresryan22/anatomy) | skill | Claude skill that explains an idea by building it as an interactive isometric figure with many small precise parts, in SVG, WebGL or 3D. |
| [machine-skill](https://github.com/AirsupHQ/machine-skill) | skill | Claude Code skill: `/machine a turbofan jet engine` researches the real machine and builds an interactive 3D physics simulation in one HTML file, plus a film to post. |
| [blender-mcp](https://github.com/ahujasid/blender-mcp) | MCP | A community MCP server that lets Claude Desktop and Claude Code control Blender 3D. Runs Python inside Blender; telemetry is on by default. |


[↑ Contents](#contents)

## Marketing

### SEO

| Name | Type | What it does |
|---|---|---|
| [claude-seo](https://github.com/AgriciDaniel/claude-seo) | plugin | A free MIT-licensed Claude Code plugin that audits technical SEO, content quality, structured data and AI search readiness. |
| [marketingskills](https://github.com/coreyhaines31/marketingskills) | skill | A free MIT-licensed collection of marketing skills for Claude Code covering conversion optimization, copywriting, SEO and analytics. |

The standalone [open-seo](#apps-agents--examples) (Semrush/Ahrefs alternative) is an app, not a plugin.

### Social Content

| Name | Type | What it does |
|---|---|---|
| [instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill) | 13 skills | Thirteen free Claude skills for running an Instagram account, including a Reel writer with 26 hook formulas and hook scoring, a niche virality ranker, caption and profile skills; nothing is posted without your approval. |
| carousel-studio ([guide](https://milleemd.com/guides/instagram-carousel-system/)) | skill (zip) | Skill (download as zip) that interviews you about your style, then renders Instagram carousels as real 1080x1350 PNGs from HTML via a headless browser. |
| [reddit-automation](https://github.com/flowkit-labs/skills) | skill | Skill that finds Reddit threads where people are shopping for what you sell and drafts helpful replies for you to review and post by hand. |
| [humanizer](https://github.com/blader/humanizer) | skill | An MIT-licensed skill that rewrites AI-sounding text to read as human, based on Wikipedia's Signs of AI writing guide. |
| [SimpleEnglish](https://github.com/AminBlg/SimpleEnglish) | skill | A free MIT-licensed skill and Claude Code plugin that makes Claude write in ASD-STE100 Simplified Technical English. |
| [xiaohongshu-mcp](https://github.com/xpzouying/xiaohongshu-mcp) | MCP | An Apache-2.0 MCP server that lets Claude Code search, read and publish on xiaohongshu.com (RedNote), including likes, favorites and comments. Publishes and comments from your account. |

### Sales Outreach

| Name | Type | What it does |
|---|---|---|
| [harvey](https://github.com/ethanplusai/harvey) | app (runs on Claude Code) | Autonomous sales agent that runs on your Claude Code subscription: finds businesses, writes specific cold emails, reads replies and keeps a local dashboard, with drafts held in an outbox for your approval. |


[↑ Contents](#contents)

## Dev

### Workflow & Planning

Add structure to how the agent plans, reviews and tests, so it stops jumping straight into code.

| Name | Type | What it does |
|---|---|---|
| [superpowers](https://github.com/obra/superpowers) | skills | Software development methodology built from composable skills: the agent asks what you want, writes a spec and implementation plan, then works through tasks with subagents, TDD and review. |
| [gstack](https://github.com/garrytan/gstack) | slash commands | Garry Tan's set of slash-command skills that turn Claude Code into a virtual engineering team: office hours, review, QA in a real browser, security audits and a ship command that opens the PR. |
| [ponytail](https://github.com/DietrichGebert/ponytail) | plugin | Plugin that makes the agent ask whether code needs to exist at all and pick the smallest complete change before writing anything. |
| [vibe-wise](https://github.com/nykooi1/vibe-wise) | plugin | Claude Code plugin that asks for your approach first, helps you weigh tradeoffs, and writes code only after you approve the design, then explains what it changed. |
| [mattpocock/skills](https://github.com/mattpocock/skills) | skills | Mattpocock's everyday engineering skills, including grill-me (relentless plan interview), grill-with-docs (builds glossary and ADRs) and improve-codebase-architecture. |
| tdd ([nulfrog/skills](https://www.skills.sh/nulfrog/skills/tdd), [superpowers](https://www.skills.sh/obra/superpowers/test-driven-development)) | skill | Test-driven development skills that enforce writing tests first in a red-green-refactor loop. |
| [everything-claude-code (ECC)](https://github.com/affaan-m/ECC) | plugin | MIT-licensed Claude Code plugin with 71 agents, 314 skills, hooks, rules and memory for planning, testing, review and verification. |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | skills | Production-grade engineering skills covering define, plan, build, verify, review and ship, driven by nine slash commands such as /spec, /plan and /build. |
| [planning-with-files](https://github.com/OthmanAdi/planning-with-files) | skill | Skill that keeps task_plan.md, findings.md and progress.md on disk, with hooks that reinject the plan so it survives /clear and context resets. |
| [beads](https://github.com/gastownhall/beads) | plugin | An open-source distributed graph issue tracker (bd) that gives Claude Code persistent task memory. |
| [skills](https://github.com/humanlayer/skills) | skill | An MIT-licensed set of Claude Code skills from HumanLayer for research, planning, implementation and pull request workflows. Some skills create pull requests. |

### Quality & Token Saving

Get better behavior from coding agents and spend fewer tokens or dollars.

| Name | Type | What it does |
|---|---|---|
| [andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | CLAUDE.md | A single CLAUDE.md with four principles (think before coding, simplicity first, surgical changes, goal-driven execution) based on Karpathy's observations on LLM coding mistakes. |
| [caveman](https://github.com/JuliusBrussee/caveman) | skill + CLI | Skill and CLI that make the agent answer tersely in caveman style and shrink logs and tool output before the model reads them, to cut tokens. |
| [TokenEconomizer](https://github.com/microsoft/TokenEconomizer) | CLI | Microsoft Research tool that learns from past sessions in a repository to cut coding-agent cost (micro-skills, tool pruning, failure-loop intervention); reports 18.4-30.9% lower mean cost on SWE-Bench. |
| [9router](https://github.com/decolua/9router) | router | Local router that connects Claude Code and other coding tools to 40+ AI providers with auto-fallback and token trimming of tool output. |
| [codegraph](https://github.com/colbymchenry/codegraph) | MCP server | Local code knowledge graph exposed over MCP that auto-syncs on every file change. |
| [gemini-mcp-tool](https://github.com/jamubc/gemini-mcp-tool) | MCP server | MCP server that lets Claude call the Gemini CLI to use Gemini's large context window for analyzing big files. |
| [CodeBurn](https://codeburn.app) | CLI | Free, open-source, local-first tracker of AI coding token usage and cost across 42 tools, broken down by model, project and task. |
| [SkillSpector](https://github.com/NVIDIA/SkillSpector) | skill | An Apache-2.0 security scanner that checks agent skills, including Claude Code skills, for prompt injection, data exfiltration and supply-chain risks before install. |
| [context-mode](https://github.com/mksglu/context-mode) | plugin | A free local Claude Code plugin and MCP server that keeps tool output out of the context window using a sandbox and SQLite full-text search. |


### Memory & Context

Stop the agent forgetting everything between sessions.

| Name | Type | What it does |
|---|---|---|
| [engram](https://github.com/Gentleman-Programming/engram) | MCP server + CLI | Persistent memory for Claude: a single Go binary with SQLite and FTS5, exposed through MCP, CLI, HTTP API and a TUI, usable with Claude Code and other MCP agents. |
| [claude-mem](https://github.com/thedotmack/claude-mem) | plugin | Plugin that automatically captures tool usage during sessions, generates semantic summaries and injects relevant context into future sessions. |
| [base](https://github.com/ChristopherKahler/base) | CLI | basemode: a Rust binary (base) that maps your workspace into a knowledge graph and wires it into Claude Code's hooks to brief the agent with relevant memory. |
| [codegraph](https://github.com/colbymchenry/codegraph) | MCP server | Local code knowledge graph exposed over MCP that auto-syncs on every file change. |
| [obsidian-skills](https://github.com/kepano/obsidian-skills) | skills | Agent skills by Obsidian's CEO for working with Obsidian, installable as a Claude Code plugin via the marketplace. |
| [Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) | plugin | Claude Code plugin that analyzes a project with a multi-agent pipeline, builds a knowledge graph of files, functions and dependencies, and offers an interactive dashboard to explore it. |
| [graphify](https://github.com/Graphify-Labs/graphify) | skill | An open-source /graphify skill for Claude Code that turns code, docs, schemas and PDFs into a queryable knowledge graph. |
| [mempalace](https://github.com/MemPalace/mempalace) | MCP | A free, local-first memory system that stores conversation history verbatim and retrieves it by semantic search through Claude Code hooks and an MCP server. |

### Browser & Web Access

Let the agent read, search, browse and scrape the web.

| Name | Type | What it does |
|---|---|---|
| [Agent-Reach](https://github.com/Panniantong/Agent-Reach) | skill + CLI | Skill and CLI that give an agent read and search access to platforms such as YouTube and Bilibili subtitles, GitHub, V2EX, web pages, Xiaohongshu and Twitter/X (experimental, needs login). |
| [playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP server | Microsoft's MCP server that gives an LLM browser automation through Playwright, using structured accessibility snapshots instead of screenshots. |
| [agent-browser](https://github.com/vercel-labs/agent-browser) | CLI | Native Rust CLI that lets an agent drive a persistent browser from the shell: snapshot a page as text with element refs, then click, fill and read again. |
| [obscura](https://github.com/h4ckf0r0day/obscura) | CLI | Open-source headless browser engine written in Rust for AI agents and scraping; runs JavaScript via V8, speaks Chrome DevTools Protocol, and can replace headless Chrome with Puppeteer or Playwright. |
| [BrowserMCP](https://github.com/BrowserMCP/mcp) | MCP | MCP server plus a Chrome extension that lets Claude control your own browser. |
| [crawl4ai](https://github.com/unclecode/crawl4ai) | MCP | Open-source web crawler and scraper with a hosted MCP server; the hosted cloud is optional, the core is self-hostable. |

### Docs Lookup

Give the agent current library documentation instead of stale training data.

| Name | Type | What it does |
|---|---|---|
| [context7](https://github.com/upstash/context7) | MCP server + plugin | Pulls up-to-date, version-specific library documentation and code examples into the agent's context so generated code matches the library versions you use. |


[↑ Contents](#contents)

## Games

### Effects & Mods

| Name | Type | What it does |
|---|---|---|
| [pixelfx](https://github.com/patch-gg/pixelfx) | library + skill | A library of 244 pixel-art effects and animations (fire, explosions, magic, weather, UI) that are each drawn from code, plus a Claude Code skill for making new ones. |
| [coop-anything](https://github.com/cranebeaker/coop-anything) | agent playbook | Agent playbook: tell Claude which single-player game you own and it researches, builds or fixes a co-op mod, tests it with bots, and packages it so friends join over Steam. |
| [awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) | plugin | 77 game-development skills (Godot, Unity, Unreal and more) in SKILL.md format, with a router skill. |
| [godot-mcp](https://github.com/Coding-Solo/godot-mcp) | MCP | Lets Claude launch the Godot editor, run projects and read debug output. |

> Needs more entries: mods, level design and asset-generation tools.


[↑ Contents](#contents)

## Career

### Job Search

| Name | Type | What it does |
|---|---|---|
| [ai-job-search](https://github.com/ai-job-search-dev/ai-job-search) | framework on Claude Code | Job application framework built on Claude Code with commands to evaluate postings, tailor your CV, write cover letters and prep interviews; MIT licensed, fork and run locally. |


[↑ Contents](#contents)

## Discovery

### Skill & Plugin Directories

Where to find more.

| Name | Type | What it does |
|---|---|---|
| [skills.sh](https://www.skills.sh/) | directory | Directory and leaderboard of agent skills, with packs, topics and audits. |
| [vercel-labs/skills](https://github.com/vercel-labs/skills) | CLI | The open agent-skills installer CLI (`npx skills add`), which installs skills from GitHub repos into Claude Code and other agents; discovery is via skills.sh. |
| [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) | list | Curated list of Claude Skills, resources and tools for customizing Claude workflows. |
| [awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) | list | Curated list of open-source skills and toolkits for making video with Claude Code (Remotion, HyperFrames, motion graphics, editing), covering 413 repos with a tested top-picks section. |
| [awesome-design-skills](https://github.com/bergside/awesome-design-skills) | list | Curated registry of 67 design-system skill files (each with SKILL.md and DESIGN.md) that you pull into a project with `npx typeui.sh pull`. |
| [wshobson/agents](https://github.com/wshobson/agents) | plugin marketplace | Marketplace of 94 plugins (202 agents, 185 skills, 105 commands) for Claude Code covering development, review, testing and infrastructure. |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | collection | Open-source library of 411 skills, plugins and agent skills for Claude Code across engineering, marketing, product, compliance and finance, with Python CLI helper scripts. |
| [top-claude-code-skills](https://github.com/selan-ai/top-claude-code-skills) | ranking | Daily-updated ranking of the top 15 Claude Code skills by GitHub stars (all time, this week, this month), each described from its own README. |
| [awesome-claude-code-skills](https://github.com/itgoyo/awesome-claude-code-skills) | list | Curated list of the top 200 GitHub repositories by stars in the Claude Code ecosystem: official tools, agent frameworks, skills, memory systems and MCP servers. |
| [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | list | Large curated list of MCP servers. |
| [claude-code-templates](https://github.com/davila7/claude-code-templates) | list | An MIT-licensed CLI and catalog of roughly 1,900 installable components for configuring and monitoring Claude Code. |
| [claude-howto](https://github.com/luongnv89/claude-howto) | list | A free MIT-licensed, example-driven guide to Claude Code with copy-paste templates for slash commands, hooks, subagents and MCP configs. |

**Security:** skills run commands on your machine, so read a skill before you install it.


[↑ Contents](#contents)

## Standalone

### Media Tools

Apps, models and datasets for video, image, audio and 3D. They run on their own and aren't Claude skills or plugins.

| Name | Type | What it does |
|---|---|---|
| [AI-Youtube-Shorts-Generator](https://github.com/Anil-matcha/AI-Youtube-Shorts-Generator) | app | Open-source Opus Clip alternative: an LLM picks highlights from long YouTube videos, Whisper transcribes, and clips are auto-cropped to 9:16 shorts. |
| [hotclip](https://github.com/xixihhhh/hotclip) | app | Free open-source local AI clipper that cuts long videos, livestream replays and podcasts into vertical 9:16 shorts with auto subtitles; publishing targets Chinese platforms. |
| [upscayl](https://github.com/upscayl/upscayl) | desktop app | Free and open-source AI image upscaler for Linux, macOS and Windows. |
| [MisoTTS](https://github.com/MisoLabsAI/MisoTTS) | model | Miso TTS 8B, an open 8-billion-parameter expressive text-to-speech model with a hosted demo and local setup via uv. |
| [VoiceStudio](https://github.com/debpalash/voicestudio) | app | Open-source (AGPL-3.0) local voice studio for cloning, designing, dubbing, dictating and transcribing voices in 646 languages, positioned as an ElevenLabs alternative. |
| [fish-speech](https://github.com/fishaudio/fish-speech) | model | Open-source text-to-speech and voice cloning model from Fish Audio. |
| [Rhubarb Lip Sync](https://github.com/DanielSWolf/rhubarb-lip-sync) | CLI | Command-line tool that automatically creates 2D mouth animation (mouth shapes) from voice recordings for games and cartoons. |
| [WhisperX](https://github.com/m-bain/whisperx) | CLI | Automatic speech recognition with word-level timestamps and speaker diarization, built on Whisper. |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | CLI | Feature-rich command-line audio/video downloader (Unlicense). |
| [NVIDIA SimReady Central](https://huggingface.co/spaces/nvidia/simready-central) | app | NVIDIA Hugging Face Space for semantic search of physics-ready OpenUSD 3D assets with RTX simulation previews. |


### Local Models & OCR

Run models on your own hardware, or read documents with AI. Not agent plugins.

| Name | Type | What it does |
|---|---|---|
| [airllm](https://github.com/lyogavin/airllm) | library | Python library for running large LLM inference on a single 4GB GPU (Apache-2.0). |
| [colibri](https://github.com/JustVugg/colibri) | inference engine | Hierarchical inference engine in C for large mixture-of-experts models: hot experts on GPU (CUDA, Vulkan), warm in RAM, cold streamed from NVMe. |
| [FreeToken](https://github.com/FlashML-org/FreeToken) | serving | Serving engine that aims to run massive models locally on a desktop (Apache-2.0). |
| [Unlimited-OCR](https://github.com/baidu/Unlimited-OCR) | model | Baidu's OCR model for one-shot, long-horizon document parsing (MIT). |

### Apps, Agents & Examples

Full products, separate agents and demo projects. Useful, but you run them yourself instead of adding them to Claude.

| Name | Type | What it does |
|---|---|---|
| [open-codesign](https://github.com/OpenCoworkAI/open-codesign) | app | Open-source (MIT) Claude Design alternative that turns prompts into prototypes, slides or PDFs; multi-model, bring your own key, local-first. |
| [open-seo](https://github.com/every-app/open-seo) | app | Open-source (MIT) alternative to Semrush and Ahrefs for SEO. |
| [jcode](https://github.com/1jehuang/jcode) | agent harness | High-performance coding agent harness written in Rust, built to run many agents in parallel with low RAM use (MIT). |
| [BettaFish](https://github.com/666ghj/BettaFish) | multi-agent app | Multi-agent public-opinion analysis assistant that collects and analyses online discussion and predicts trends (GPL-2.0). |
| [hermes-agent](https://github.com/NousResearch/hermes-agent) | agent | Nous Research's open-source agent that grows with you (MIT). |
| [paperclip](https://github.com/paperclipai/paperclip) | app | Open-source (MIT) app for managing teams of AI agents at work. |
| [OpenMausBot](https://github.com/milind-soni/OpenMausBot) | bot | Open-source Grok Bot alternative with a virtual machine the bots can use (Apache-2.0). |
| [Claude-of-Duty](https://github.com/mshumer/Claude-of-Duty) | example | Demo of a Call of Duty-style first-person shooter in Three.js built from a single prompt (MIT). |
| [clauding](https://github.com/nishaj0/clauding) | app | Discord Rich Presence for Claude Code and the Claude desktop app: status, model and live token counts. |
| [craft-anything](https://github.com/storytold/craft-anything) | app | Open-source (MIT/Apache-2.0, early alpha) desktop app and MCP server that studies a website, app or game, then has Claude Code build your own version and check it against the original. |
| [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | list | 100+ open-source AI agent, agent-skill and RAG app examples, including Claude and MCP ones. |
| [mcp-use](https://github.com/mcp-use/mcp-use) | app | TypeScript framework for building MCP servers and MCP apps. |
| [notebooklm-py](https://github.com/teng-lin/notebooklm-py) | skill | Unofficial Python API, CLI and skill for Google NotebookLM; needs a NotebookLM account. |
| [whatsapp-mcp](https://github.com/lharries/whatsapp-mcp) | MCP | An MIT-licensed MCP server that connects your personal WhatsApp account to Claude so it can search, read and send messages. Sends messages from your WhatsApp account. |


[↑ Contents](#contents)

## Planned (empty)
Writing, data & analytics, testing & QA, DevOps, security, documentation, finance, education, and more SEO entries.


[↑ Contents](#contents)

## Types used in tables
`skill` · `plugin` · `MCP` (server the agent calls) · `CLAUDE.md` (rules file) · `collection` / `list` · `app` · `model`


[↑ Contents](#contents)

## Security
Entries are checked for what they claim to do, but **they are not security-audited or guaranteed safe**. Skills, plugins and MCP servers can run commands, read your files and send data out. Read the source before you install anything, check what permissions it asks for, and take extra care with anything that sends messages, posts online or spends money. Scanners such as [SkillSpector](https://github.com/NVIDIA/SkillSpector) can help, but they don't replace reading it yourself.


[↑ Contents](#contents)

## Contributing
Add a row to the right section above. See [CONTRIBUTING.md](CONTRIBUTING.md).
