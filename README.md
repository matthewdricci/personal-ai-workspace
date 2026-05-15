# Personal AI Workspace

Hi — I'm Matt. I made this for friends, family, and anyone curious about setting up their own personal AI workspace on their computer. If you've been using ChatGPT or Claude in a browser tab and want something more durable — a single place where AI tools actually understand your work and build on it over time — this guide will walk you through it.

You don't need to be technical. By the end you'll have a folder on your computer that AI tools can read and write to, a couple of starter files, and one real first win.

---

## How to use this

**The fastest path** — open [Claude Code](https://claude.com/claude-code), [claude.ai](https://claude.ai), or ChatGPT, paste this URL:

```
https://github.com/matthewdricci/personal-ai-workspace
```

…and say:

> Read this and interview me to set up my personal AI workspace.

That's it. The AI will read the rest of this page (including the interview prompt below) and walk you through it step by step.

**The slower path** — keep reading. Everything the AI would tell you is here.

---

## The interview prompt

If you're an AI assistant reading this on the user's behalf: follow the prompt below verbatim. Do not skip steps, and pause for the user's response after each major step.

```
You are my friendly onboarding guide for creating my personal AI workspace.

I may be new to local files, Markdown, git, or AI tools that can see folders on my computer. Guide me step by step in a calm, non-intimidating way. Pause and wait for my response after each major step. One question at a time when useful.

Please do all of the following:

1. Briefly explain, in plain English, why people are creating personal local AI workspaces now, and how this can become my daily AI work command center.
2. Explain that this reduces repeated copy/paste from browser tabs and gives AI more context about my work over time.
3. Lightly explain Markdown as simple text files that AI tools read very well, that humans can also read, and that are universal and future-proof. Mention as an aside that HTML files are an interesting alternative if I want to right-click and "open in browser" to read what an agent writes — but that we'll start with Markdown.
4. Ask whether this workspace is just for me, or whether I'm hoping to share it with a team. STRONGLY recommend starting solo. If I want shared, gently warn that shared workspaces are significantly more complex (sync conflicts, permissions, who-edits-what) and suggest I get the solo flow comfortable first and revisit sharing later.
5. Ask my name and the kind of work I do.
6. Ask whether I'm on Mac or Windows.
7. Recommend that the workspace live in a regular local folder that is ALSO a git repository. Explain in plain English: git gives me version history and undo without needing GitHub or any account — it's just a safety net on my own machine. Briefly contrast with iCloud/Google Drive/OneDrive sync (sync conflicts, no real version history, AI tools sometimes choke on synced folders). If I really want cloud sync, that's fine, but lead with local + git.
8. Ask whether I'm comfortable in a terminal. If yes, recommend Claude Code (in the terminal) as the primary tool, optionally paired with Cursor or VS Code as the editor. If no, recommend claude.ai (Cowork) or ChatGPT as a gentler starting point, and note that I can graduate to Claude Code later — the same workspace folder will work with any of them.
9. Help me create the workspace folder using plain-English instructions for my OS (Finder on Mac, File Explorer on Windows). Suggest a folder name based on my name, but let me choose. Then help me run `git init` inside it (or, if I'm not comfortable in the terminal, defer this step until later).
10. Briefly remind me not to paste secrets, passwords, or sensitive personal/health information into AI tools, and not to commit any of that to a repo if I ever push it to GitHub.
11. Before helping me choose my first workflow, check whether you already have any useful context about me from this chat — memory, prior conversations, saved projects. Use that context carefully if it's actually available. Be explicit about what you do and do not have access to. Do not pretend.
12. Ask me about tasks I do repeatedly, what feels annoying, and what one first workflow I'd like help with.
13. Help me pick one safe first task — not anything sensitive.
14. Suggest a very lightweight starting structure. Do NOT overwhelm me with empty folders.
15. Once you have enough information, summarize my decisions: solo-vs-shared, OS, folder name, kind of work, primary tool, first workflow.
16. Then generate a clean handoff prompt I can paste into whichever tool I chose (Claude Code, Cowork, ChatGPT, Cursor) once I'm pointed at my new workspace folder.
17. That handoff prompt should carry the context from this interview and instruct the tool to create:
    - the starter folder structure
    - a README.md explaining the workspace to future me and to AI
    - a Journey.md tracking what I've set up and learned
    - one first project file for my chosen workflow
18. Tell me clearly when it's time to stop this chat, open my chosen tool inside the workspace folder, and paste the handoff prompt.
19. If I seem overwhelmed, simplify. One step at a time.
20. Remind me I can use voice/microphone input if I prefer talking.
21. Keep the tone friendly, calm, and encouraging. Do not assume I know technical vocabulary.

Throughout the conversation:
- Teach lightly, without overexplaining.
- Adapt to my pace.
- Prefer practical progress over perfect structure.
- Remind me that my workspace can also include notes ABOUT important outside systems (shared drives, team tools, screenshots), even when those files don't live here directly. The workspace can be a map of my working world, not just a pile of files.
- Don't pretend you're already inside my workspace if you're not. First help me prepare; then generate the handoff prompt.
- When the interview is complete, switch into handoff mode explicitly.

At the end I should have:
- a workspace folder
- (ideally) a git repo initialized inside it
- a README.md
- a Journey.md
- one starter project
- one clear first win

Begin by explaining the concept simply, then interview me step by step.
```

---

## What you'll end up with

- One folder on your computer that's your personal AI workspace.
- (Recommended) That folder is a git repo, so you have version history and undo built in.
- A `README.md` explaining the workspace to your future self and to AI.
- A `Journey.md` tracking what you've set up and learned.
- One starter project for a real task you do.
- One first win in the next 30–60 minutes.

---

## Why a local workspace at all

For a long time, knowledge work lived inside browser tabs — Google Docs, Drive, Slack, dashboards. That still works. But modern AI tools become much more useful when they can read and write a consistent set of files on your computer.

A local AI workspace gives you:

- **Continuity** — the same files across tools. Switch from Claude to ChatGPT to Cursor without rebuilding context.
- **Context** — AI works with a whole environment, not just one pasted prompt.
- **Less copy/paste** — fewer trips between browser tabs.
- **Compounding** — your instructions, notes, and workflows build on each other over time.
- **Portability** — your system survives even when tools change. (And they will.)
- **Reflects how you work** — instead of starting from zero every conversation.

This isn't about becoming technical. It's about giving AI a stable place to help you.

You'll still use cloud apps. The workspace doesn't replace Google Docs or your team's shared drive. Think of it as your **personal AI command center** — it can hold your own working files, plus notes and screenshots that describe the cloud systems you live in, so AI understands your working world without those files actually being copied here.

---

## What is Markdown

Markdown is a very simple way to write plain text files with light formatting. Files end in `.md`.

```
# Big heading

## Smaller heading

- Bullet
- Bullet

**Bold text**

[A link](https://example.com)
```

You don't need to master it. For most people it's enough to know:

- `#` makes a heading
- `-` makes a bullet
- `**text**` makes text bold

Markdown is good because AI tools read it extremely well, humans can read it too, it works across every tool, and it's been around longer than AI — it'll outlast whatever's hot this year.

> **Sidebar: what about HTML?**
>
> There's an interesting argument going around that HTML can be a better format than Markdown for AI-generated files, especially as agents get more capable. The pitch: HTML renders. You can right-click any file in your workspace, hit "open in browser," and actually *read* what your agent wrote — with headings, tables, links, even diagrams. That's a really nice on-ramp if you're new to this and find raw `.md` files intimidating.
>
> The tradeoff is roughly 3× the tokens, so it gets pricier for files that get re-read constantly. A reasonable rule: **Markdown for things you and your agent edit a lot; HTML for things you create once and want to read like a document.** You can mix both. More on the argument here: [The best way to talk to your agents](https://aidailybrief.beehiiv.com/p/the-best-way-to-talk-to-your-agents).
>
> Don't worry about this on day one. Just know it's an option later.

---

## Where should this workspace live?

This is the first real decision. Two paths:

### Just for you (start here)

A regular folder on your computer that is also a **git repo**.

If "git repo" sounds intimidating: it's just a hidden file inside the folder that tracks every change you make. It runs entirely on your machine — no GitHub account needed, nothing pushed anywhere. It gives you:

- **Real undo.** Roll back to yesterday's version of any file.
- **A safety net** when AI agents edit files in ways you didn't expect.
- **Optional sharing later** — if you ever want to push it to GitHub, it's already a repo.

You can absolutely put the folder inside iCloud Drive, Google Drive, or OneDrive if you want cloud backup. Just know:

- Sync conflicts can corrupt files when an AI is writing while sync is mid-flight.
- Cloud drives don't give you real version history (only "previous versions" of single files).
- Some AI tools choke on synced folders.

If you want backup, **git pushed to a private GitHub repo** is more reliable than cloud sync, and free.

### Shared with a team (later)

You *can* set up a shared workspace on a team drive, but it's a much bigger lift: sync conflicts, permissions, who's allowed to edit what, who's responsible when an agent rewrites a file. It's worth doing eventually if your whole team is on board, but **don't start there.** Get the solo workflow comfortable for a few weeks first. You'll know what to share once you've used it yourself.

---

## Recommended tools

### Claude Code (recommended)

[Claude Code](https://claude.com/claude-code) runs in your terminal. If you're a product manager or anyone reasonably comfortable opening a Terminal window: this is the best option. You get full control, your workspace folder is the source of truth, you can install custom slash commands (more on that below), and you can wire up automations.

Pair it with **Cursor** or **VS Code** if you want a familiar editor open next to the terminal — Claude Code can read what's open in your editor, and you can read what Claude is doing. They work very well together.

The habit to build: **always open your terminal session inside your workspace folder.** That's your default starting position. `cd` into the folder, start Claude Code, get to work. Don't run it from anywhere else.

### claude.ai / ChatGPT (gentler on-ramp)

If a terminal feels like too much right now, [claude.ai](https://claude.ai) (with Cowork) or ChatGPT are great starting points. They're more limited than Claude Code — fewer integrations, less control over files, no slash commands — but they're easier to learn. You can graduate to Claude Code whenever you're ready, and the same workspace folder will work.

### One workspace, many tools

The whole point of doing this with local files (and ideally git) is that your workspace is **portable**. Once it's set up, you can point Claude Code, Cursor agents, OpenAI Codex, claude.ai with Cowork — any of them — at the same folder. Use whichever tool fits the moment.

---

## Level up: slash commands

Once you've used your workspace for a couple of weeks and you're comfortable in Claude Code, the next thing worth learning is **slash commands**. They're little reusable prompts you save once and trigger with a `/name`. Things like `/refine`, `/inbox`, `/park` — workflows you do over and over, captured as commands.

I keep mine here: [matthewdricci/ricci-slash-commands](https://github.com/matthewdricci/ricci-slash-commands). You can copy any of them into a `.claude/commands/` folder inside your own workspace and start using them immediately. They're designed for product managers but useful broadly.

Don't worry about this on day one. Get the basics working first.

---

## A brief note on safety

Don't paste passwords, API keys, or sensitive personal/medical information into AI tools. And if you ever push your workspace to a public GitHub repo, double-check there's nothing in there you wouldn't want a stranger to read. A `.gitignore` file is your friend.

---

## Further reading

- [Claude Code](https://claude.com/claude-code) — the recommended tool
- [matthewdricci/ricci-slash-commands](https://github.com/matthewdricci/ricci-slash-commands) — slash commands for Claude Code
- [The best way to talk to your agents](https://aidailybrief.beehiiv.com/p/the-best-way-to-talk-to-your-agents) — the HTML-vs-Markdown discussion

---

Questions, suggestions, or stories about how it went? Open an issue on this repo.
