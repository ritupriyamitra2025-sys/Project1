# Instruction Log (date-wise)

**U-n** = owner's instruction · **A-n** = AI's understanding / action · newest at the bottom.
Raw files live in `01-Original-Instructions/`. Paths are relative to this folder.

---

## 2026-10-07

**U-1** — Uploaded the project plan (`01-Original-Instructions/2026-10-07_U-1_Project-Plan_ORIGINAL.docx`, text: same name `.txt`). The plan sets out folders 1–14 and the end goal. Instruction: read it, explain the understanding in 20–30 lines, do not build anything until "start". Folder 14 is the only thing allowed before "start".

**A-1** — Read the whole plan and gave a summary. Listed four limits:
- The cloud session cannot see F:\ or C:\.
- The AI does not start by itself when a file arrives.
- Deadlines and case law must be verified.
- Copying the old data will take several sessions.

Asked: which court system, how to reach the files, and how many voice notes exist.

**U-2** — Courts: any USA court (trial, appeal, supreme), Canada, India. Files: the owner can put them in a PC folder or any drive. Voice notes: 19.

**A-2** — Rules design: general rules plus one rule file per court where a case exists, each deadline with a rule number and source. Recommended running Claude Code on the owner's PC. The Dropbox connector cannot upload Word or PDF files. GitHub is not suitable for large or private files. Next voice note = 20.

**U-3** — "Do you have any question for me?"

**A-3** — Asked:
1. Is anything due in 2–3 weeks?
2. Will you use the Claude desktop app on your PC?
3. Are any papers sealed or confidential?
4. When will you delete the old folders?
5. Is OCR of scanned PDFs OK?

**U-4** — "Can you see and access all the folders in the plan?"

**A-4** — Checked: **no**.
- The cloud session has no F:\ or C:\.
- Dropbox is blocked (email not verified).
- Google Drive is blocked (limited permission).
- The repo is empty.

Only the uploaded plan has been read.

**U-5** — Opened the same session in the desktop app.

**A-5** — Checked: the session still runs in the cloud. To reach F:\, start a **new local session** in the desktop app on `F:\`. Gave a hand-off note to paste there.

**U-6** — Answers:
- Yes, a filing is due in the next 2–3 weeks.
- No papers are sealed or confidential.
- The old folders will be deleted manually, only after the project is proven.
- OCR is OK.

**A-6** — Priority: the urgent filing first, the full build after. Asked for the filing details (court, date, type, draft or not). Updated the hand-off note.

**U-7** — Correction: **copy, not move**. Copy only important files.

**A-7** — Agreed: copy only, never move or delete. Important files are the CPs, appeal files 1–170, trial and Supreme Court filings, orders, quick references, audio, and useful rules. Duplicates, old drafts, and temporary or empty files are skipped. A copy/skip list goes to the owner for approval before any copying.

**U-8** — "Did you read the project plan file?"

**A-8** — Yes, all of it. Corrected my own wording ("move" → "copy"). Noted that `START-HERE.md` and the master file list are AI suggestions, not part of the plan. Asked whether folder 1 keeps the original after processing.

**U-9** — The folder structure is only a suggestion; the AI may change it to reach the end goal. Relative paths are a must. Nothing is built until "start", but scanning is allowed. Asked why folder 14 was not created, since it was meant to be made before "start".

**A-9** — Admitted the miss: the plan allows folder 14 before "start" ("this is the only file which you can put inside that"). Created folder 14 in the project repo (the cloud session cannot write to F:\):
- `README.md`
- `01-Original-Instructions/` (original `.docx` plus `.txt`)
- `02-Project-Understanding.md` / `.docx`
- `03-Instruction-Log.md`

The owner copies this folder to `F:\6th October -2026\14.ProjectMaking`, or the local session pulls it from the repo.

---

### Open items
- [ ] Urgent filing details: court, due date, document type, draft or not.
- [ ] Folder 1: keep the original after processing, or empty it?
- [ ] Approve or reject the AI suggestions: `START-HERE.md`, the master file list.
- [ ] Start a local Claude Code session on `F:\` and confirm folder access.
- [ ] Owner to say **"start"**.
