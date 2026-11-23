*English · [ภาษาไทย](README.th.md)*

# Team Notes Hub — interface demo

### ▶ [Open the demo](https://olay097056.github.io/team-notes-hub-demo/)

A walkthrough of **Team Notes Hub**, a small shared web app for a team's
manuals, notes and files — Finder-style folder sidebar, always-on search bar,
and shared-password login. The live team instance and its real content remain
private; this page is a standalone preview.

**Everything here is synthetic.** This page is a static, read-only preview of
the interface. Every folder, note, tag and snippet of text was invented to look
the way the real tool does — nothing on this page is real team content and
nothing connects to a live system.

## What the demo covers

**Folder sidebar** — the Finder-style navigation with folders, tags and Trash.
Click any folder to see its notes, any tag to filter across folders, or Trash
to see the soft-delete list.

**Search** — the always-on search bar that filters across every note by title
and body text. Use `Ctrl/⌘ K`, then the arrow keys and Enter to move through
suggestions.

**Note view** — a sample rich-text note rendered the way the editor stores it:
checklists, tables, code blocks, quotes and headings.

**Editor preview** — a sample of the current formatting toolbar, outline,
attachment row, and Preview/Print controls. `New Note` and `Edit preview` open
this static editor view; Save and upload actions explain that nothing is stored.

## About the real app

Next.js (App Router) + Tailwind CSS, PostgreSQL, and Docker Compose for local
and LAN deployment (with optional Caddy HTTPS for public use). A single shared
password gates access — no per-user accounts — because the PRD calls it a
small, trusted-team tool. Daily automated backups are the recovery path for the
no-undo editor. The note body uses Tiptap v3 for rich content.

The app source is in the public [team-notes-hub repository](https://github.com/Olay097056/team-notes-hub). The live team instance and its content are not connected to this demo.
