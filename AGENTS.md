# AGENTS.md

Conventions for any AI agent working in this repository.

## What this repo is — and is not

This is the **public interface demo** of `team-notes-hub`, which is a private
team notes / manuals / shared-files web app (Next.js + Postgres) used inside a
company. The app itself stays private; this repo is a self-contained,
hand-rolled static preview so people can see what the interface looks like
without the code or the real data.

**Nothing from the private repository is copied here.** No source files, no
configuration, no secrets, no real content. All note titles, bodies, folder and
tag names in `index.html` are synthetic/invented. If a fact would help the demo,
restate it in general terms — do not pull real manual text or real file names.

**The honesty ribbon at the top stays.** A viewer must be able to tell within
one screen that this is a synthetic demo. Do not remove it, shrink it into a
footnote, or soften the wording.

## The demo itself

- Single `index.html`. No framework, no build step — served straight off
  GitHub Pages.
- The layout mirrors the real app: top search bar, Finder-style folder
  sidebar with tags and Trash, a note list, and a rich-text note view (task
  lists, tables, code blocks).
- Interactivity is client-side only: opening folders, tags, Trash, and notes,
  plus a live search filter. Nothing persists and nothing writes.

## Git

- **Never `git push` unless the human explicitly asks for it in that message.**
- **Never `git add -A` / `git add .` blindly.** Stage named paths.
- Commit author identity comes from global git config (`NW <olay097056@gmail.com>`).
- Do not rewrite history that already exists on `origin/main`.

## Docs

- `README.md` and `README.th.md` are kept in sync. Updating one means updating
  the other.
