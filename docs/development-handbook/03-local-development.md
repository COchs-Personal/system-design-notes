# Local reading and maintenance on NixOS

Git and a Markdown-capable editor are sufficient. There is no dependency manifest, local application server or pinned Nix environment required to read the notes. Open the root index and follow a few representative links. Use exact case-sensitive paths on NixOS. A local renderer may be useful, but choosing one is a tooling decision, not an existing repository command.

```bash
git status --short --branch
git ls-files
rg -n '<img|!\[|\]\(' Readme.md '04. Rate Limiter' '12. Chat System'
git diff --check
```

The search helps inspect references and image usage. It does not verify that every remote URL still works or that external articles remain current. This handbook describes the committed notes; no remote source verification was performed for its claims. When relying on a linked article for a new technical recommendation, read the primary source and record when it was checked.

Check local links relative to the file containing them. A root link and a chapter's image link have different starting directories. If renaming a chapter, search all incoming references before moving it. Avoid bulk whitespace or capitalization changes mixed with conceptual edits; they make it harder to see whether the technical explanation changed.

No container is required. If future maintenance introduces a renderer in a container, it must use Podman and a reproducible, documented environment. Do not add a complex publishing stack merely to read static notes. Routine hosted CI is disabled under workspace policy; use appropriate local checks and retain human review before publishing.

A documentation test can establish that local files resolve and Markdown structure is sound. It cannot establish that a distributed algorithm tolerates failures. Keep those evidence levels clear when describing validation in a PR.
