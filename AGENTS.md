# Project instructions

## Publishing to the live website

- This repository publishes `main` to `https://aadil815.github.io/` through GitHub Pages.
- The user has granted standing authorization for Codex tasks in this repository to commit and push task-specific changes directly to `main` when the user asks to publish, deploy, make changes live, or otherwise clearly requests a live update. Do not require a pull request or ask for an additional publishing confirmation in those cases.
- Before publishing, inspect `git status` and the relevant diff. Stage only the files belonging to the requested change unless the user explicitly confirms the entire working tree. Preserve unrelated work from other tasks.
- Fetch `origin/main` before committing or pushing and reconcile newer remote commits without overwriting them.
- GitHub CLI is installed at `C:\Program Files\GitHub CLI\gh.exe`. If `gh` is not found through `PATH`, use that absolute path instead of reporting that GitHub CLI is unavailable.
- GitHub authentication is stored in the Windows keyring. Verify it with `& 'C:\Program Files\GitHub CLI\gh.exe' auth status`; if sandboxed credential access fails, retry through the approved normal-system-access path.
- Publish with an intentional commit and `git push origin main`. Never force-push.
- After pushing, wait for the `pages build and deployment` workflow to finish and verify the affected public URL returns successfully and reflects the new content.
