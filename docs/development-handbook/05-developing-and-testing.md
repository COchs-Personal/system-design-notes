# Developing better notes

## Recipe: clarify a rate-limiter boundary case

Open `04. Rate Limiter/Readme.md`, locate the fixed-window explanation and its edge-burst image, and add an original small timeline with a chosen window size and request limit. Show requests just before and just after the boundary and count which are allowed. Explain what property the example demonstrates and which alternative changes it. Keep this as an explanatory example, not a benchmark of a missing implementation.

Review the same language in the image caption and surrounding comparison. Check that “strict,” “approximate,” “burst,” and “rolling” have clear meanings. If proposing an actual implementation later, it belongs in an explicitly scoped code project with concurrency and failure tests, not hidden inside an educational paragraph.

## Recipe: improve an ID design explanation

In `07. Unique-Id Generator/Readme.md`, connect the example bit allocation to the stated capacity and time horizon. Clarify worker identity and clock behavior with source-backed reasoning. Distinguish uniqueness, numerical order, causality and strict global order: these are different promises. Avoid an unsupported statement that clock synchronization alone solves every rollback or failover case.

Keep worked arithmetic local and reproducible. State units, epoch and assumptions. A reader should be able to recompute the example without needing to trust an unexplained large number. Link to a primary source when adding a technical claim, but do not copy long passages from it.

## Recipe: repair navigation and images

Find the exact referenced path, including case and spaces. Inspect whether the link is Markdown or HTML and whether it is relative to the current chapter. Repair the smallest broken reference and search for other references to the same file. Open the chapter in the intended renderer and inspect the figure and its alt text. Preserve original images and attribution unless a deliberate replacement is supported and licensed.

When exporting to Word or PDF, check that tables, numbered steps, code examples and image captions remain readable. A successful export command is not visual QA. The editable Markdown should remain the maintainable source, with exports synchronized rather than independently rewritten.

## Evidence for a reviewable change

A good PR explains the reader problem, the corrected explanation, source support and local link/render checks. It should not claim tests of a nonexistent deployed system. Keep changes to one concept or navigation problem where possible. Use a topic branch, target the canonical primary branch, and retain human merge authority.
