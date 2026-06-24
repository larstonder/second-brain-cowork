---
name: capture-to-note
description: Turn something the user read or watched into a structured Learning note in their Obsidian vault, no terminal or downloads required. Use when the user shares an article URL, pastes article/newsletter/email text, shares a YouTube URL, or pastes a transcript and wants it captured, summarized, turned into notes, or "saved to my second brain". Triggers on a pasted URL or pasted text combined with requests to "capture", "summarize", "make a note", "extract key points", "save this", or "what does this say".
---

# Capture to note (Cowork, no terminal)

Turn a source the user gives you into a `learning` note in their vault. Built for Claude Cowork and non-coders: it works from **text the user pastes** or a **URL**, never from downloads or a terminal. An article is the default source; a YouTube video is an optional one.

## Getting the source text in

Work with whatever the user gives you, in this order of preference:

1. **Pasted text** (article, newsletter, long email, their own notes): use it directly.
2. **An article/web URL:** try to read the page directly. If you cannot fetch it, ask the user to open the page, select all (Cmd/Ctrl+A), copy, and paste the text in. Copying page text always works.
3. **A YouTube URL (optional):** ask the user to paste the transcript. They can get it from the video's **... ▸ Show transcript**, or from a browser extension, then paste it. If a YouTube-transcript connector (MCP) happens to be available, you may fetch it directly instead.

If you have only a bare URL and cannot read it, do not guess the contents. Ask for the text.

## Workflow

1. **Confirm the basics:** the source (URL and/or title) and, for a video, the channel/author.
2. **Read the source.** For long text, summarize in passes. Do not invent facts that are not in the source.
3. **Ask for the angle.** A personalized extraction beats a generic summary:
   > "Who is this for, and what are you focused on right now?" (e.g. a consultant prepping a workshop, a parent planning a trip).
4. **Draft the note** using `Templates/Learning.md` and the conventions in the vault's `CLAUDE.md`:
   - Frontmatter: `type: learning`, `created:` today's date in `DD.MM.YYYY`, `source:` the URL, `author:` the site/author/channel, `status: draft`, plus a tag like `#source/article` or `#source/video`.
   - Sections: **Summary**, **Key Takeaways** (numbered), **Quotes** (only real quotes from the source), and **How I'll Apply This** (specific, not generic).
   - Add `[[wiki links]]` only where a connection to existing notes is genuinely real. Search the vault first. Zero links is fine if nothing relates yet. Never write a paraphrased claim next to a link whose target does not exist.
5. **Confirm with the user, then save** the note in `Learning/`.
6. Suggest opening **Graph View** in Obsidian to see the new note connect to the vault.

## Notes

- Quote only what is actually in the source. If you are paraphrasing, make it clearly a summary, not a quote.
- Auto-generated YouTube transcripts lack punctuation and speaker labels; infer from context and do not invent facts.
- This skill never needs a terminal, an install, or an API key. The reliable path is always: paste the text.
