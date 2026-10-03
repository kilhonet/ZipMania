# ZipMania

**A fast, lightweight free archiver for Windows that opens 50+ archive formats and compresses to 7Z · ZIP · TAR.**

English · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> This document is a translation. If anything differs, the [Korean version](README.ko.md) is authoritative.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Source](https://img.shields.io/badge/source-Apache%202.0-lightgrey)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/zipmania?lang=en)

![ZipMania screenshot](images/zipmania-en.webp)

## Overview

ZipMania is an archiver focused on one thing: opening and creating archives. It reads 50+ formats including ZIP, RAR, 7Z, EGG, ALZ and ISO, and creates archives in **7Z · ZIP · TAR**.

Open an archive and you get a folder tree on the left and a file list on the right. Pick just the files you need and extract them, or drag them straight into Explorer. Images are previewed without extracting. Double-click a file to open it in its associated program, and an archive inside an archive opens in a new window.

The Explorer right-click menu gives you one-click actions such as "Extract Here" and "Compress to *name*.zip", and a command-line tool (`zm.exe`) is included for backup scripts and external programs like Total Commander. No ads, no bundled software.

## Features

- **Opens 50+ formats** — ZIP, ZIPX, JAR, RAR, 7Z, EGG, ALZ, TAR, GZ, BZ2, XZ, ZST, ISO, IMG, WIM, DMG, MSI, RPM, DEB, CAB, CBZ, CBR and more.
- **Compresses to 7Z · ZIP · TAR** — five compression levels, passwords, 7Z file-name encryption, split archives.
- **Fast ZIP** — a dedicated ZIP engine handles ZIP compression and extraction.
- **Only what you need** — extract selected files, drag them to Explorer, or double-click to open them directly.
- **Archives inside archives** — double-click to open them in a new window.
- **Image preview** — JPG, PNG, GIF, WebP, SVG and more, shown in the lower-left pane without extracting.
- **Archive editing** — add files to or delete files from 7Z, ZIP and TAR archives.
- **Verify · Scan** — a CRC table shows whether the archive is damaged, and inner files can be scanned by your Windows antivirus (AMSI).
- **Clean up after compressing** — verify the archive when done and delete the sources only if it passes.
- **Explorer right-click menu** — Extract Here, Extract to *name*, Compress to *name*.zip, Compress each separately, Extract each to own folder.
- **Command line** — `zm.exe` (console) and `ZipMania.exe` (progress window) for compress, extract, list and test. Accepts both 7-Zip and Bandizip option styles.
- **Dark/light theme, 9 languages** — follows Windows by default, or choose your own.

## Download / Installation

| Package | Link |
|---|---|
| Installer | [Download](https://down.kilho.net/zipmania?lang=en) |
| Portable (ZIP) | [Download](https://down.kilho.net/zipmania?lang=en&nosetup) |

ZipMania can be used as a portable app: unzip anywhere and run `ZipMania.exe`. Settings are stored in `settings.toml` next to the executable, so they travel with it on a USB stick.

## Usage

### Getting started

**Extracting**

1. Double-click an archive, open one with **[Open]** in ZipMania, or drop it onto the window.
2. Browse the folder tree on the left and the file list on the right. Select files and click **[Extract]**.
3. In the **Extract** window choose the destination folder. Use the quick links on the left (Desktop, Documents, Downloads, …) or the folder tree; right-click an empty spot to create a new folder.
4. Under **Files to extract** choose **All files** or **Selected files**, then click **[OK]**. Progress, speed and time remaining are shown; when finished, **[Open folder]** takes you to the result.

**Compressing**

1. Click **[New Archive]** on the toolbar, or drop files and folders onto the ZipMania window.
2. The **New Archive** window lists them. Add more with **[Add Files]** / **[Add Folders]** or by dropping them in.
3. Set the **File Name** (save location), **Format** (7Z · ZIP · TAR), and if needed **Set Password**, **Split**, the **After** actions and the **Method**.
4. Click **[Start]**. When finished, **[Open folder]** or **[Close]**.

To do it straight from Explorer, use the right-click menu — see "How to…" below.

### The window

| Toolbar button | What it does |
|---|---|
| **Open** | Open an archive |
| **Extract** | Extract the open archive (or only the files you selected) |
| **New Archive** | Pick files and folders and create a new archive |
| **Add Files** / **Delete Files** | Put files into or remove them from the open archive (7Z · ZIP · TAR only) |
| **Verify** | Check the archive for damage (CRC) |
| **Scan** | Scan inner files with your Windows antivirus (files under 10 MB) |
| **Flat View** | Show every file in one list with its full path, ignoring folders |
| **Settings** | Theme, language, extraction defaults, file associations, Explorer menu |

- **Folder tree (upper left)** — click a folder to show its files on the right.
- **Preview (lower left)** — appears when a single image file is selected.
- **File list** — Name · Size · Packed Size · Type · Modified. Click the Name, Size or Modified header to sort; drag the borders to resize columns.
- **Status bar** — item count, number and size of selected files, packed size and ratio.
- Drag the divider to resize the tree and list. Window size and maximized state are restored next time.

### How to…

**Extract straight from Explorer**
Right-click an archive to get the ZipMania entries.
- **Extract Here** — extracts into the archive's own folder without asking. Turn on **Close window** in the progress window to have it close as soon as it finishes.
- **Extract to "name"** — creates a new folder named after the archive and extracts into it. Best for archives with many files.
- **Extract with ZipMania…** — opens the window where you pick the destination and options.
- **Open with ZipMania** — look inside first.

With **several archives selected**, **Extract Here** extracts them one after another, and **Extract each to own folder** puts each archive in a folder of its own name.

**Compress straight from Explorer**
Right-click files or folders.
- **Compress to "name.zip"** — creates a ZIP right there without asking. One folder gives the folder's name; several items give the current folder's name. If the name is taken, a number is added: `name (2).zip`.
- **Compress with ZipMania** — opens the window to choose format, password, split and so on.
- **Compress each separately** — makes one ZIP per selected item, named after it. Handy for archiving several folders individually.

**Pull just a few files out of an archive**
Three ways:
- Select the files (Ctrl/Shift for several) and click **[Extract]** → **Files to extract: Selected files**.
- Right-click the selection → **Extract Selected Files**.
- **Drag the selection to Explorer or the desktop** — it is extracted right there.

**Open a file inside an archive without extracting**
Double-click it or press Enter; it opens in its associated program (documents in your editor, videos in your player). Right-click → **Run File** does the same. Temporary copies are cleaned up when you close ZipMania.

**An archive inside an archive**
Double-click it and it opens in a **new window**. You can keep several windows open and switch between them.

**Flip through photos inside an archive**
Select an image file (JPG · PNG · GIF · BMP · WebP · ICO · SVG · TIFF · AVIF) and a preview appears in the lower left. Use the arrow keys to move through them. Images over 32 MB show a notice instead of a preview.

**Deep folders make files hard to find**
Turn on **[Flat View]** on the toolbar: folders are flattened and every file is listed with its path. Sort by name, size or date to find the biggest or newest files at once. Click again to return to folder view.

**Password-protected archives**
A password prompt appears when you open one. A wrong password asks again; a correct one is remembered for that archive, so preview, open and extract do not ask again. If a protected file turns up during extraction, you are asked then; leave it blank and only that file is skipped while the rest continues.

**Compress with a password**
In the **New Archive** window click **[Set Password]** and type it.
- With **7Z** you can also turn on **Encrypt file names** — without the password no one can even see what is inside.
- **ZIP** accepts letters and digits only. A non-ASCII password shows a warning and will not start — switch to 7Z or use an ASCII password.
- **TAR** does not support passwords.

**Send a big file by email or messenger**
Under **Split** pick 10 MB · 25 MB · 100 MB · 700 MB · 1 GB · 4 GB, or choose **Custom…** and type something like `700M` or `4GB`. The archive is saved as `name.7z.001`, `.002`, … (7Z · ZIP). The recipient puts the parts in one folder and opens or extracts **only the `.001` file**.

**Delete the originals after compressing to free up space**
Under **After** turn on **Verify archive** and **Delete sources**. The sources are deleted only when every file was stored and the verification passed, so a bad archive never costs you the originals.

**Compress several folders separately**
Put the folders in the **New Archive** window and turn on **Compress each item into its own archive**. Each folder gets an archive of its own name, next to it. It is the same as Explorer's **Compress each separately**, but here you can also choose the format and a password.

**Faster or smaller**
**Method** has five levels: **Store (no compression)** · **Fast** · **Normal** · **High** · **Maximum**. To just bundle already-compressed photos or videos, **Store** is fastest; for documents and source code that shrink well, **High** or **Maximum** pays off. For the smallest result use the **7Z** format (the default).

**Add or remove files in an existing archive**
With a 7Z · ZIP · TAR archive open:
- Click **[Add Files]** or drop files onto the window — answer Yes to "Add N file(s) to …?".
- Select files and click **[Delete Files]** or right-click → **Delete Files**.
Other formats (RAR, EGG, …) cannot be edited, so the buttons are disabled.

**Check whether a downloaded archive is intact**
Click **[Verify]**: each file's expected and actual CRC are compared and shown in a table. Damaged or partially downloaded archives are caught before you extract them.

**Check whether a downloaded archive is safe**
**[Scan]** hands the inner files to your Windows antivirus (AMSI) without extracting them. Files of 10 MB or more are skipped, and an antivirus with real-time protection must be running. The result lists each file as Clean · Threat · Skipped.

**A file with the same name already exists when extracting**
You are asked per file: **Overwrite** · **Skip** · **Rename**. Turn on **Apply to all remaining files** to use the same answer for the rest.

**Extraction scattered files all over the folder**
**Create a subfolder named after the archive** is on by default, so files go into a folder named after the archive. To extract directly, turn it off in the **Extract** window or in **Settings → Extraction**, or use Explorer's **Extract Here**.

**Delete the archive and open the folder when done**
In **Settings → Extraction** turn on **Delete the archive after successful extraction**, **Open destination folder after extraction** and **Close the extract window after extraction**. They can also be changed in the Extract window each time. The archive is deleted only when extraction succeeded.

**Make double-click open archives in ZipMania**
Check the extensions in **Settings → File Association**. If another program already owns an extension, it shows **[Not applied]**; click it to open Windows' default-app picker and choose ZipMania. When ZipMania opens an archive and shows "Make ZipMania the default app for … files?" at the top, you can switch right there.

**ZipMania is missing from the right-click menu**
In **Settings → Explorer Menu** turn on **Add ZipMania compress/extract to the Explorer right-click menu**. On Windows 11 it appears in the main menu; if you do not see it, look under **Show more options** (Shift+F10).

**Open the archive's folder / delete the archive**
Right-click an empty spot in the list for **Open Containing Folder** and **Delete Archive**. After checking the contents you can delete an archive you no longer need without leaving ZipMania.

**Drive the list with the keyboard**
Arrow keys · Page Up/Down · Home/End to move, Shift for a range, Ctrl-click to add single items, **Ctrl+A** to select all, Enter to enter a folder or open a file, Esc to close the password or report dialog.

**Dark mode and language**
Both follow Windows by default. In **Settings → General** choose the theme (System · Light · Dark) and the language (한국어 · English · 日本語 · 中文 · Русский · Italiano · Français · Español · العربية); changes apply immediately. The Explorer menu uses the same language.

**Backup scripts and Total Commander**
Two executables are provided.
- **`zm.exe`** — prints to the console. cmd, PowerShell and batch files wait for it to finish and receive an exit code (0 success / 1 warning / 2 error).
- **`ZipMania.exe`** — runs the same commands with a **progress window**. Suited to places without a console, such as Total Commander.

```
<exe> a|c [options] <archive> <inputs...>   compress (a adds to an existing archive)
<exe> x|e [options] <archive> [items...]    extract (x keeps folders, e files only)
<exe> bx  [options] <archives...>           extract each archive into a folder of its own name
<exe> l   [options] <archive>               list
<exe> t   [options] <archive>               integrity test
```

| Option | Meaning |
|---|---|
| `-l:0..9` / `-mx9` | Compression level |
| `-fmt:zip\|7z\|tar` / `-t7z` | Format (defaults to the archive extension) |
| `-v:700M` / `-v700m` | Volume size |
| `-p:password` / `-ppassword` | Password |
| `-o:folder` / `-ofolder` | Destination folder |
| `-target:auto\|name\|none` | Extract into a subfolder named after the archive (`auto` = only when there is more than one top-level item) |
| `-aoa` `-y` / `-aos` / `-aou` | On a name clash: overwrite / skip / save as `name (2)` |
| `-testdst` | Verify the archive after compressing |
| `-delsrc` / `-sdel` | Delete the sources when verification passes |
| `-date` | Replace `%Y %y %m %d %H %M %S` in the file name with the current time |

Examples:

```
zm c -l:9 -fmt:7z -testdst -delsrc -date "backup_%y%m%d_%H%M.7z" "D:\Work"   dated 7Z backup, verify, then delete sources
zm a -mx9 -psecret backup.7z D:\Work                                       7-Zip style, add to an existing archive
zm x -o:D:\Out -target:auto backup.7z                                      extract into a folder named after the archive
zm bx a.zip b.7z                                                            extract into a\ and b\ respectively
zm l backup.7z.001                                                          list the first part of a split archive
```

Run `zm` with no arguments for help. Inside a batch file write `%` as `%%`. For a Total Commander user command, set the command to `zm.exe` and the parameters to `c -l:9 -fmt:7z -aou -testdst -delsrc -date "%T%S %y%m%d_%H%M".7z "%P%S"` to compress the selected items into a dated 7Z in the opposite panel's folder.

## Configuration

Everything is changed in **Settings** (rightmost toolbar button) and saved immediately. **[Reset]** restores all defaults.

| Category | Item | Default |
|---|---|---|
| General | Theme (System · Light · Dark) | System |
| General | Language (System + 9 languages) | System |
| Extraction | Create a subfolder named after the archive | On |
| Extraction | Delete the archive after successful extraction | Off |
| Extraction | Open destination folder after extraction | Off |
| Extraction | Close the extract window after extraction | Off |
| File Association | Extensions opened in ZipMania by double-click (zip · 7z · rar · tar · gz · tgz · bz2 · xz · egg · alz · cbz) | Associated by the installer |
| Explorer Menu | Add ZipMania compress/extract to the Explorer right-click menu | Enabled by the installer |

The **Close window** and **Open folder** checkboxes in the New Archive and Extract windows remember your last choice.

## Requirements

- Windows 10 or Windows 11, **64-bit**
- No additional runtime or components are needed.
- Internet access is used only to check for a new version. Compression and extraction work offline.

## Updates

ZipMania does **not** update itself. It checks for a new version at startup and only lets you know; new versions are published manually after internal verification and announced on the [ZipMania page](https://kilho.net/zipmania). See the [update policy notice](https://en.kilho.net/archives/notice/2940).

## Building from Source

The source is public at [github.com/newkilho/ZipMania](https://github.com/newkilho/ZipMania) (Rust 1.88 or later). The archive engine, `crates/zipmania-archive`, builds and tests from the repository alone:

```
cargo test -p zipmania-archive
```

The application (`app/`) depends on an in-house GUI engine and shared libraries outside the repository, so the executable cannot be built from the repository alone.

## Contributing

Bug reports and suggestions are welcome via GitHub issues or the [forum](https://kilho.top/forum/qna).

## License

The ZipMania program is **Freeware**. Use it anywhere — at home, at work, in schools and government offices — and redistribute it freely in unmodified form.

The source code is licensed under the **Apache License 2.0**; the reusable crates under `crates/` are available under MIT or Apache-2.0 at your option. The names "ZipMania" and "집매니아" and the logos and icons are trademarks of Kilho.net and are not covered by the license — distribute modified versions under a different name and icon. Open-source components including 7-Zip's `7z.dll` (LGPL) are listed in `THIRD-PARTY-NOTICES.txt` in the repository.

## Links

- Website: <https://kilho.net/zipmania>
- Source: <https://github.com/newkilho/ZipMania>
- Forum: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
