GPU Database - GitHub Pages Fixed Build
=======================================

This build embeds the full databases directly inside index.html:
- 560 GPUs
- 1,141 games

This prevents the empty-database problem caused by failed fetch() paths,
repository subfolders, cached JSON files, or opening the site from a different
GitHub Pages base path.

UPLOAD INSTRUCTIONS
-------------------
1. Extract this ZIP.
2. Upload the CONTENTS of the extracted folder to the root of the GitHub branch
   or /docs folder configured for GitHub Pages.
3. Make sure index.html is directly in the published root, not one folder deeper.
4. Keep the assets folder beside index.html.
5. After publishing, hard-refresh the browser with Ctrl+F5.

The external gpus.json and games.json files are still included for editing and
backup, but the live page no longer depends on fetching them.
