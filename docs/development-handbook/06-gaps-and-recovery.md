# Gaps, troubleshooting and preservation

| Symptom | What to inspect | Safe repair |
|---|---|---|
| Root chapter link fails | Exact path, capitalization and encoded spaces | Correct the reference to the real directory; search incoming links before renaming |
| Image missing locally | Chapter-relative path and actual asset file | Restore or correct that asset reference; retain descriptive text |
| Figure looks different in PDF | HTML styling support and export layout | Adjust supported formatting and visually review the result |
| Two chapters appear contradictory | Different assumptions, scale or consistency goals | State those assumptions before deciding whether either explanation is wrong |
| External article disappeared | Original title, author, URL and citation context | Find a legitimate original/archive or mark unavailable; do not silently substitute unrelated advice |
| Reader expects executable examples | File inventory and chapter scope | Explain that this is a notes collection; propose code work separately |

The first improvement priority is a local reference audit across all 28 chapters and their images, including case-sensitive paths. Acceptance is reproducible local link checks plus representative rendering. The second is clearer assumptions and source dates for numerical/product examples. Acceptance is a reader being able to distinguish a worked design from a current operational fact. The third is consistent captions, terminology and accessibility across HTML-heavy and Markdown-heavy chapters.

The root index contains a doubled slash in the rate-limiter directory link and a doubled space in the digital-wallet directory name. These are concrete navigation details to inspect before normalizing anything. A doubled slash may be tolerated by one renderer while failing elsewhere; a directory rename requires updating all references, not merely the displayed title.

Back up the Git repository, including image assets and history. External web pages are not preserved by cloning these notes. An export is useful for reading but cannot replace editable chapter sources and original attribution. If a diagram or note is accidentally removed, compare the known revision in a clean checkout and restore only the intended file while preserving unrelated edits.

No user accounts, database, service ports or live study-session state exist here. Closing the editor is sufficient to end ordinary use. The important recovery criterion is readable, attributable material with working local navigation, not the health of an imagined application.
