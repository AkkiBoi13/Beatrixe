# Changelog

Beatrixe organizes PDF and EPUB downloads into your library on Windows. Downloads are on the [releases page](https://github.com/AkkiBoi13/Beatrixe/releases).

## 0.1.6 — 14 November 2026

Fixes from a full review of the app and the browser companion. None of the problems could move, overwrite or delete a book without your approval.

- **Undo can be tried again.** If Undo failed, for example because the book was open in a reader, every later Undo also failed. Now you can try again once the cause is gone.
- **No stuck History entries after startup.** If your library drive was not available when Beatrixe started, an entry could stay "needs review" for good. Beatrixe now waits and checks again at the next start. A move between drives that is waiting for your cleanup approval stays waiting instead of becoming a conflict.
- **Scans never offer existing folders for removal.** A folder Beatrixe cannot read, or one beyond the 2,000-folder scan limit, is kept and never ticked for removal. The scan dialog says how many folders could not be read, and top-level folders are always read first.
- **Personal documents stay private.** Bank statements, receipts, ID scans and study notes in your library are never learned as book titles, so they are never sent as examples with Organize with AI. Only names recognised as books are ever sent as AI examples, and titles learned by earlier versions are checked again before anything is sent.
- **Folder editor:** typing a new folder's name no longer takes over another folder's subfolders, and renaming a folder carries only its own subfolders.
- **Browser helper updates:** the setup script now replaces an earlier Beatrixe registration, even from a deleted folder, so updating into a new folder works. BROWSER-SETUP.md has an update section.
- History no longer stops accepting moves after 4,096 entries; it keeps the latest 4,096 and says so.
- History names a partial copy left by an interrupted move between drives, so you can find and delete it.
- The analysis worker runs only inside its memory-limited sandbox, from its first instruction.
- The tray stays responsive while a large batch of moves is approved.
- In the scan dialog, unticking a folder gives its subfolders back their own choice, and rule counts say when they include subfolders.
- Learned titles are kept correctly when you undo a second copy, or when a move finishes while a scan is open, and every folder gets fresh titles even past the 5,000-title limit.
- Moves no longer each re-read the whole library for the new-folder reminder.
- Browser companion: requests are served side by side, so one slow request no longer makes others say "Beatrixe is not running". The last-download note is never stale and says the folder watcher may still find a file that was not sent.
- Folder errors name the folder and say what is wrong.

## 0.1.5 — 14 November 2026

- The new-folder reminder counts only folders a scan can add. With the folder list full at 64, it no longer keeps asking about folders that don't fit.
- **Browser companion: honest status.** The popup says whether Beatrixe is connected, has no download folder yet, is busy, needs attention or isn't running, and whether the browser helper is missing. It shows the extension and Beatrixe versions and warns when they differ.
- **Busy retries.** When Beatrixe is busy moving files, the extension keeps trying for about 15 seconds instead of once.
- **Site labels.** A site you list also covers its subdomains and downloads started from its pages, so mirror and CDN downloads get the label. Only the name you entered is sent.
- **No 256-download limit.** After 256 downloads in 30 minutes, Beatrixe forgets the oldest label instead of refusing new ones.
- The extension's version now matches Beatrixe's, and the setup guide links to the latest release.
- Older browser helpers and extensions keep working with this release. The popup says when the helper is out of date; install the helper and extension from the same release as Beatrixe.

## 0.1.4 — 14 November 2026

- **Scan your library.** A new Library folders panel at the top of Settings. Scan library folders reads your folders, two levels deep, and the names of the books already in them. Scan another folder copies the structure of a different folder. A dialog shows new folders, folders already in use, and folders that are gone, which you can remove one by one. Nothing changes until you apply it, and a scan never moves, renames or creates files.
- **Suggestions from your own sorting.** Review suggests the folder holding books with similar titles, and Beatrixe learns from every move you approve. On a manual sort of 511 books, the right folder was suggested for 333 books, against 179 using folder names alone.
- **New-folder reminder.** Settings and Review say when your library has folders Beatrixe doesn't use yet, with Scan now and Not now.
- **Subfolders.** The folder editor shows a tree, and Add subfolder adds a folder under any folder. It is created on disk only when you approve a move into it.
- **Organize with AI** also sends up to 3 example titles from each folder; the confirmation says so.
- Scanning keeps automatic rules on for folders that still exist, and keeps AI suggestions you already paid for.
- After 0.1.4 saves a scan, earlier versions can't open the Beatrixe profile.

## 0.1.3 — 14 November 2026

- **Better book detection.** Book names only recognizes Z-Library, Anna's Archive, libgen, ISBN and "Title (Author)" names, and hides tickets, receipts, ID scans and worksheets. Rows show a cleaned title; hovering a name shows why it counts as a book.
- **Your own folders.** Settings offers the folders already in your library as categories, or suggests folders from the books found.
- **Organize with AI on Review.** Suggests a destination for checked rows or all book names, after a confirmation that shows what is sent and how many requests it uses. Suggestions only fill in destinations; moves still need Preview and Approve. A run can be stopped, and suggestions are kept.
- **Automatic AI explains itself** when it is approved but waiting, for example because monitoring is off.
- After 0.1.3 saves AI suggestions, earlier versions can't open the Beatrixe profile.

## 0.1.2 — 13 November 2026

- Review opens in **Book names only**; **All PDFs and EPUBs** shows every supported document.
- Optional AI organization with OpenAI, Gemini or Anthropic using your own API key, an approved source folder and a daily request limit. AI moves appear in History and can be undone.

## 0.1.1 — 13 November 2026

- First public Windows release: review suggested destinations, approve moves, and find or undo completed moves in History.
- Browser companions for Chrome, Edge and Firefox with a Windows native host.
