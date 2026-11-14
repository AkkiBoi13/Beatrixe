# Changelog

Beatrixe organizes PDF and EPUB downloads into your library on Windows. Downloads are on the [releases page](https://github.com/AkkiBoi13/Beatrixe/releases).

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
