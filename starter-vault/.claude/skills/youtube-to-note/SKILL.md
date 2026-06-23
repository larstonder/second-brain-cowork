---
name: youtube-to-note
description: Turn a YouTube video into a structured Learning note in the user's Obsidian vault, no terminal or downloads required. Use when the user shares a YouTube URL or pastes a video transcript and wants notes, a summary, key takeaways, or learnings captured. Triggers on YouTube links (youtube.com/watch, youtu.be) or a pasted transcript combined with requests to "summarize", "make a note", "extract key points", "notes from this video", "capture this", or "what does this video say".
---

# YouTube to note (Cowork, no terminal)

Turn a YouTube video into a `learning` note in the user's vault. This skill is built for Claude Cowork and non-coders: it relies on the user **pasting the transcript**, not on downloading anything.

## Two ways to get the transcript

**If a YouTube-transcript connector (MCP) is available**, prefer it: when the user gives a YouTube URL, fetch the transcript directly through the connector tool, then continue to the workflow below. No copy-paste needed.

**Otherwise, use the paste flow (the default, always works).** If the user gave only a URL and no transcript, ask them to fetch it from YouTube, it takes a few seconds:

1. Open the video on youtube.com.
2. Under the video, click **... (more) ▸ Show transcript**.
3. (Optional) Toggle timestamps off in the transcript panel.
4. Select the transcript text, copy it, and paste it into the chat.

If the transcript is in another language, that is fine, work in that language.

## Workflow

1. **Confirm the basics** with the user: the video URL, and ideally the channel/author and a one-line "why this video".
2. **Read the pasted transcript.** Strip timestamps and obvious filler in your own reading. If the transcript is very long, summarize in passes.
3. **Ask for the angle.** A personalized extraction beats a generic summary:
   > "Who is this for, and what are you focused on right now?" (e.g. consultant prepping a workshop, parent planning a trip).
4. **Draft the note** using `Templates/Learning.md` and the conventions in the vault's `CLAUDE.md`:
   - Frontmatter: `type: learning`, `created:` today's date in `DD.MM.YYYY`, `source:` the URL, `author:` the channel name, `status: draft`, plus a `#source/video` tag.
   - Sections: **Summary**, **Key Takeaways** (numbered), **Quotes** (only real quotes from the transcript), and **How I'll Apply This** (specific, not generic).
   - Add `[[wiki links]]` only where a connection to existing notes is genuinely real. Search the vault first. Zero links is fine if nothing relates yet. Never write a paraphrased claim next to a link whose target does not exist.
5. **Confirm with the user, then save** the note in `Learning/`.
6. Suggest opening **Graph View** in Obsidian to see the new note connect to the vault.

## Notes

- Auto-generated transcripts lack punctuation and speaker labels; infer from context and do not invent facts.
- Quote only what is actually in the transcript. If you are paraphrasing, make it clearly a summary, not a quote.
- This skill never needs `yt-dlp`, a terminal, or any install. If the user cannot find the transcript option, they can paste the video's description or key points instead.
