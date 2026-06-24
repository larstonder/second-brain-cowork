# START_HERE.md

> **For the participant's agent (Claude Cowork).** If you are a human reader: open Claude Cowork on the `starter-vault/` folder and tell the agent *"Read `START_HERE.md` and help me get going."*

You are helping someone who does **not** code build their own AI-driven second brain during a ~1 hour workshop. The stack is fixed: an **Obsidian vault** (the `starter-vault/` folder) plus **Claude Cowork** (this app). There is no quiz and no choice of backend, so do not offer alternatives like Notion or SharePoint. Keep everything inside the vault folder.

**Be Norwegian-friendly.** Participants are Norwegian. If they write in Norwegian, reply in Norwegian. These docs are in English, but their notes will likely be Norwegian.

**Confirm before writing.** Summarize what you are about to create or change, and wait for a yes before writing to disk.

---

## Step 1: Confirm the setup (2 min)

Check, and help fix anything that is missing:

1. **The vault is open in Obsidian.** Ask the participant to confirm they opened the `starter-vault` folder as a vault in Obsidian and can see the folders (`Learning`, `Meetings`, `Notes`, ...).
2. **This Cowork project points at the vault folder.** You should be able to read and write files under it.
3. **The conventions are loaded.** Read `starter-vault/CLAUDE.md` and confirm out loud that you understand: the folder structure, the required frontmatter, the `DD.MM.YYYY` date format, and the "always use `[[wiki links]]`, only when the link is real" rule.

If you cannot read the vault files, stop and help the participant give this project access to the `starter-vault` folder before going on.

---

## Step 2: Write the first real note (10 min)

Ask the participant to pick one small thing they actually want to remember. Examples: a book or article they read, a meeting from yesterday, something they learned this week, or a person they want to keep track of (from their own memory, not scraped from LinkedIn).

Then, together, create the note. You must:

1. Pick the correct folder for the type (`Learning/`, `Meetings/`, `Notes/`, `Personal/People/`, ...). See the table in `starter-vault/CLAUDE.md`.
2. Start from the matching template in `starter-vault/Templates/`.
3. Fill in frontmatter with today's date in `DD.MM.YYYY` format.
4. Add `[[wiki links]]` only where a connection is genuinely real. Zero links is fine if nothing in the vault truly relates yet. Never write a paraphrased claim next to a link whose target does not exist.
5. Confirm the content with the participant before saving.

Then have them look at the note in Obsidian: the frontmatter shows up as a **Properties** panel, and **Graph View** (`Cmd/Ctrl+G`) shows the note as a dot. It is lonely now. That changes in the challenges.

---

## Step 3: Hand off to the challenges

Point the participant at `docs/06-challenges.md`:

- **Challenge 1, Capture:** turn an article (or any pasted text; a YouTube transcript optionally) into a structured `Learning` note.
- **Challenge 2, Customize:** make one tilpasning of your own (a small skill or a saved instruction).

The crew will call time between challenges.

---

## Guardrails for you (the agent)

- **Confirm before writing.** Summarize, then wait for sign-off.
- **Never invent content.** If the participant has not given you input for a note, ask for it.
- **Respect the frontmatter and linking rules** in `starter-vault/CLAUDE.md`. Links only when the connection is real. Never pad to hit a count, and never write an agent-authored paraphrase next to a link whose target does not exist.
- **Stay in scope.** This is a 1 hour, non-coder workshop. If asked about enterprise rollout, MCP servers, terminals, or scraping LinkedIn, say it is out of scope for today and point at `docs/07-going-further.md`.
- **When the participant is stuck, suggest they flag down a crew member on the floor.** That is what the crew is there for.
