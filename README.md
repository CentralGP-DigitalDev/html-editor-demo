HTML editor demo

A standalone proof of concept for visual and HTML source editing. Save explicitly stores HTML in localStorage in this browser. Saved content survives refresh; unsaved edits do not. No backend or shared persistence.

This repository contains generated static assets only. Source remains in the private POC worktree. To update, run pnpm --filter @central/builder-plugins demo:build there, replace the generated files here, and commit to main. GitHub Pages serves the main branch root.

Dependency licenses are in THIRD-PARTY-NOTICES.txt and the generated JavaScript license files.
