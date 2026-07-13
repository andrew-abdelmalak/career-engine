# CLAUDE.md — for an AI agent working in this repo

This file is read by Claude Code, Cowork, or any Claude-powered dev tool opened on this folder. It's about the *repo*, not about how Career Engine behaves once it's live as a Claude Project — that behavior is entirely defined by `Project Setup.md`, which you should treat as a separate, already-finalized document.

## What this repo is

Career Engine is a portable Claude Project template: a set of files someone pastes/uploads into their own Claude Project so it can generate tailored CVs and cover letters, draft LinkedIn copy, and answer career questions from their personal knowledge base. It's built to be reused as-is — a friend forking this repo should get equivalent quality to the original author without editing any rules file, only their own knowledge base.

## Folder map

| Path | Purpose |
|---|---|
| `README.md` | Public landing page — what this is, how to set it up |
| `Project Setup.md` | The literal text to paste into a Claude Project's Name/Description/Instructions fields |
| `Context-Files/` | Upload these into the Project's knowledge (Files) section as-is |
| `Knowledge Base File Example/` | A structural template for a new user's own knowledge base — reference only, not uploaded to the live Project |
| `Mine (not in GitHub)/` | The original author's actual personal knowledge base — real data, never committed, never referenced when editing shared files |
| `Internal/` | This file. Not for end users. |

## Hard rule: personal data never leaves `Mine (not in GitHub)/`

That folder holds one specific person's real facts. Never copy content from it into `Context-Files/`, `README.md`, `Project Setup.md`, or any file that ships to other users — that's exactly the hardcoding this project has been through multiple passes to remove. If you're helping set up `.gitignore`, confirm that folder is excluded before any commit.

The same rule applies in reverse to anyone else's data: if a user shares their own CV or knowledge base with you while using this repo, treat it the same way — theirs to keep local, never something you commit or paste into a shared file.

## Editing `Context-Files/`

Every file in here must stay generic. Two tests before committing a change to any rules file (`CV - Rules.md`, `Cover Letter - Rules.md`, `LinkedIn - Rules.md`):

1. **No hardcoded personal examples.** A rule can describe a pattern ("flag a usable quote if the knowledge base has one"); it can never name a specific person's employer, quote, or entry. If removing the specific person from a sentence breaks it, the sentence is wrong.
2. **No assumptions about the knowledge base's structure.** Say "check what the knowledge base says about X," never "check the table in section 2.1" — a user's file might not have a section 2.1.

Cross-file references between rules files (e.g. `Cover Letter - Rules.md` pointing at `CV - Rules.md`) are only earned where a real structural dependency exists, not added for completeness.

If you rename any file in `Context-Files/`, grep the whole repo for the old name first — `Project Setup.md` and the other rules files reference each other by exact filename, and a stale reference is a silent failure, not an error.

## Editing `Project Setup.md`

This is the one file that actually runs, every message, inside a live Career Engine Project. Read it in full before touching it — it's dense on purpose, every line is there because an earlier, more verbose version was cut down. Don't restate something one tag already guarantees inside another tag.

## Helping someone bootstrap a knowledge base from just a CV

Someone using this repo may only have a CV, not a written-out personal history. That's a fully supported starting point, not a degraded one:

1. Read whatever they give you (CV, LinkedIn export, transcript) in full.
2. Restructure it into `Knowledge Base File Example/Knowledge Base - Example.md`'s section layout — Personal Info, Education, Experience, Certifications, Leadership, Languages — using their actual content. This alone is enough to use Career Engine.
3. Optionally, offer to go deeper: ask clarifying questions per entry (context, what they actually did, how, what happened) and write the fuller narrative version in their words. Only do this if they want to invest the time — never invent detail they didn't give you, and never treat the compressed version as incomplete or wrong.
4. Their finished file is theirs to keep locally (their own equivalent of `Mine (not in GitHub)/`) — it doesn't belong in a shared or forked copy of this repo.
