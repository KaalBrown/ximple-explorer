# Ximple Explorer 0.9.17 preview

This version fixes sidebar repainting and makes the browsing interface more compact and responsive.

- **Clean sidebar opening and closing.** File lists and headers repaint together, preventing stale columns and duplicated text. Sidebar and pane-layout choices save after a short idle interval; closing the app still saves the final choices.
- **Closed sidebars stay closed.** Background navigation and row-height updates preserve their hidden state, and scrollbar updates are batched until the rows are ready.
- **Less work on each click.** Common preferences save only the setting that changed. List, Folder icons and Thumbnail switches keep reusable thumbnail artwork and save only that folder's view. Choosing the current view again skips unnecessary work.
- **Responsive menus for large selections.** Edit and file right-click menus use loaded selection metadata while retaining command availability, color states and saved customization.
- **Immediate return from search.** Closing a folder search restores its retained listing, filters, selection and scroll, then checks for changes in the background. Locations without a usable retained listing load normally in the background.
- **More working room.** The compact header groups tabs, the sidebar toggle and the Folder menu, followed by navigation and filtering. Header and footer spacing return 40 logical pixels to the file area. Edit, View and the default right-click menu group related actions together; custom menu order and visibility are preserved.

Cross-pane tab dragging, device browsing, Start menu integration and file shortcuts remain available. Existing settings and scan history are preserved. The preview remains free and is for Windows 11 x64.

## Download

- [XimpleExplorer.exe](https://github.com/KaalBrown/ximple-explorer/releases/download/v0.9.17/XimpleExplorer.exe): standalone app.
- [XimpleExplorer.exe.sha256](https://github.com/KaalBrown/ximple-explorer/releases/download/v0.9.17/XimpleExplorer.exe.sha256): SHA-256 checksum for the app.
- [XimpleExplorer-0.9.17-preview-win11-x64.zip](https://github.com/KaalBrown/ximple-explorer/releases/download/v0.9.17/XimpleExplorer-0.9.17-preview-win11-x64.zip): portable folder with the app, README, release notes, third-party notices and licenses.
- [ZIP checksum](https://github.com/KaalBrown/ximple-explorer/releases/download/v0.9.17/XimpleExplorer-0.9.17-preview-win11-x64.zip.sha256): SHA-256 checksum for the package.

Save the standalone executable to a normal local folder and run it, or extract the ZIP and open **XimpleExplorer.exe**. The executable is unsigned. Keep Windows security protections enabled and report any block or warning.

An existing Start menu shortcut or default-folder registration can still point to an older managed copy. Open 0.9.17 and choose **Help > Add Ximple to Start menu...** or **Help > Make Ximple the default folder explorer...** again to update the corresponding integration. Launching the new preview alone does not update those registrations.
