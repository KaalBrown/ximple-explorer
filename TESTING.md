# Try Ximple in about 10 minutes

Use Windows 11 on an x64 PC. Start with disposable copies of your files, and keep originals elsewhere. This is a development preview, not a backup utility.

## 1. Download and open

Download the ZIP and its `.sha256` file from the [preview release](https://github.com/KaalBrown/ximple-explorer/releases/tag/v0.9.12-preview). Extract the ZIP into a normal local folder and run `XimpleExplorer.exe` beside its documentation and licenses.

The publisher is currently unsigned. Leave Windows security protections enabled. If your system blocks the application, report the warning rather than disabling protection.

Optional download-integrity check in PowerShell, from the folder containing the ZIP:

```powershell
Get-FileHash -LiteralPath '.\XimpleExplorer-0.9.12-preview-win11-x64.zip' -Algorithm SHA256
```

Compare the result with the accompanying checksum file. A matching checksum confirms integrity, not that the program is safe.

## 2. Make a small test workspace

Create two folders named `Ximple Test A` and `Ximple Test B`. Put copies of a few documents and pictures in A, plus one subfolder containing more copies. Open A in one pane and B in the other. Keep these copies separate from important files.

## 3. Try these tasks

| Task | What to check |
|---|---|
| Browse folders, then use Back, Forward and Up | Locations and selections remain understandable. |
| Open and switch tabs in both panes | Each pane retains its own folders and navigation. |
| Switch between side-by-side and stacked panes | Controls and filenames remain readable. |
| Copy sample files from A into B | Originals remain in A; copies open correctly in B. |
| Copy the same names again | Conflict choices are clear and the chosen result is correct. |
| Rename a sample file with F2 | The pointer becomes an I-beam; clicking positions the caret; dragging selects text. Enter confirms and Escape cancels. |
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

For the initial release check, use a separate Windows 11 x64 installation or fresh VM without Ximple settings or development tools. Download the published ZIP there rather than transferring an existing extracted copy. Complete the table above and record any download, launch or security warning. Report failures as failures, including security blocks.

Suggested result format:

```text
Ximple version:
Windows version/build and x64 confirmed:
Fresh Windows installation / separate PC:
Downloaded from the public release:
ZIP extracted and app launched:
Any Windows/security warning (exact wording):
Navigation and tabs:
Copy and conflict handling:
Rename with mouse / Enter / Escape:
Search and Space view:
Theme/scaling and restart:
Problems or comments:
```
