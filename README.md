HTML editor demo

A standalone proof of concept for visual and HTML source editing. Load a sample, edit it, and see the live preview. Refresh resets edits to the default sample. No persistence or backend.

This repository contains generated static assets only. Source remains in the private POC worktree. To update, run pnpm --filter @central/builder-plugins demo:build there, replace the generated files here, and commit to main. GitHub Pages serves the main branch root.

Dependency licenses are in THIRD-PARTY-NOTICES.txt and the generated JavaScript license files.

QA candidate published 2026-11-11

Source revision: db0bfdab. This candidate adds responsive property dialogs, collapsed image sections, edge-aware properties tabs, clearer conversion notes, and focused validation feedback. Shared editor logic was simplified.

Verification: 296 automated tests passed. Typecheck, lint, the production demo build, and six real-browser layout checks passed. Image and table tabs were also checked at each edge. The existing webpack bundle-size warning remains.

QA should exercise representative production content, native clipboard paste from the applications authors use, mouse and touch selection/dragging, keyboard navigation, table Apply/Cancel/Escape/undo, images and links, and repeated Visual/HTML switches. Check that unsupported content remains intact and conversion requires confirmation. Compare the live preview and source after edits. Please include the sample or minimal HTML, browser/device, steps, expected result, and screenshot when reporting a defect.

Scope: this is a standalone demo, not the installed Builder plugin. Refresh resets content; there is no save backend. Real Builder save/reopen, external host updates, actual role permissions, physical mobile devices, and other browser engines still require QA. The preview disables scripts and does not load destination-site CSS. No production site or Builder configuration was changed by this publication.
