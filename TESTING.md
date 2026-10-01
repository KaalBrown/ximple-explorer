# Try Ximple in about 10 minutes

Use Windows 11 on an x64 PC. Start with disposable copies of your files, and keep originals elsewhere. This is a development preview, not a backup utility.

## 1. Download and open

Download `XimpleExplorer.exe` and `XimpleExplorer.exe.sha256` from the [0.9.15 preview release](https://github.com/KaalBrown/ximple-explorer/releases/tag/v0.9.15). Save the executable to a normal local folder and run it. No installer is needed.

The publisher is currently unsigned. Leave Windows security protections enabled. If your system blocks the application, report the warning rather than disabling protection.

Optional download-integrity check in PowerShell, from the folder containing the executable:

```powershell
Get-FileHash -LiteralPath '.\XimpleExplorer.exe' -Algorithm SHA256
```

Compare the result with the accompanying checksum file. A matching checksum confirms integrity, not that the program is safe.

## 2. Make a small test workspace

Create two folders named `Ximple Test A` and `Ximple Test B`. Put copies of a few documents and pictures in A, plus one subfolder containing more copies. Open A in one pane and B in the other. Keep these copies separate from important files.

## 3. Try these tasks

| Task | What to check |
|---|---|
| Browse folders, then use Back, Forward and Up | Locations and selections remain understandable. |
| Open, close, reopen and switch tabs in both panes, including folders with images or videos | Tab changes stay responsive and each pane retains its own folders and navigation. |
| Drag a tab from one pane's tab bar to a position in the other pane's tab bar | The insertion marker shows the destination; the tab arrives with its folder and navigation history. Moving the only tab leaves a fresh tab in the source pane. A pane already holding ten tabs rejects another. |
| Focus a file list and type the beginning of a name | Selection jumps to the matching file or folder and wraps through the list. |
| In Folder icons or Thumbnails, right-click the background and change Sort by | Name, date, type, size and ascending/descending choices reorder the visible items. |
| Switch between side-by-side and stacked panes | Controls and filenames remain readable. |
| Expand This PC in both sidebars and right-click its heading | Network and Connected devices can be hidden or shown separately in each sidebar. Drives and WSL entries remain available, and the choices survive restart. |
| If Windows exposes a network share, WSL distribution or connected phone/storage provider, open it in either pane | Supported locations navigate inside Ximple; Refresh devices retries discovery. Record unavailable or unsupported actions accurately. |
| Expand and collapse several sidebar groups | The list responds promptly without jumping to an unexpected position. |
| Copy sample files from A into B | Originals remain in A; copies open correctly in B. |
| Copy the same names again | Conflict choices are clear and the chosen result is correct. |
| Rename a sample file with F2 | The pointer becomes an I-beam; clicking positions the caret; dragging selects text. Enter confirms, Escape cancels, and the confirmed new name appears promptly. |
| Search subfolders for a filename | Expected matches appear; opening a result reaches the correct file. |
| Scan the sample workspace in Space view | Folder totals and categories make sense; opening a location works. |
| Switch themes and try your normal display scaling | Text, icons, selection and rename fields remain readable. |
| Close and reopen Ximple | Open folder paths, tabs and your chosen preferences return. |

Do not test permanent deletion on anything you need. Undo is limited to eligible operations in the current session and is not a general recovery guarantee.

## 4. Send a result

[Open a bug report or feedback form](https://github.com/KaalBrown/ximple-explorer/issues/new/choose), or reply to the community announcement where you found Ximple.

Include:

- Ximple version, from Help > About.
- Windows version/build, from Settings > System > About.
- Your display scaling if reporting a visual issue.
- Local disk, USB, network share or cloud-provider folder, if relevant.
- Exact steps, expected result and actual result.
- Optional screenshot with private information removed.

“Everything worked” is useful too: tell us which tasks you completed and the type of machine/storage used. No personal files or complete system reports are required.

## Clean-machine release check

For the initial release check, use a separate Windows 11 x64 installation or fresh VM without Ximple settings or development tools. Download the published executable there rather than transferring an existing copy. Complete the table above and record any download, launch or security warning. Report failures as failures, including security blocks.

Suggested result format:

```text
Ximple version:
Windows version/build and x64 confirmed:
Fresh Windows installation / separate PC:
Downloaded from the public release:
EXE downloaded and app launched:
Any Windows/security warning (exact wording):
Navigation and tabs:
Tab drag between panes:
Copy and conflict handling:
Rename with mouse / Enter / Escape:
Search and Space view:
Device visibility, theme/scaling and restart:
Problems or comments:
```
