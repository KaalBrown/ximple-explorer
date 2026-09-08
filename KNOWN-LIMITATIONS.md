# Development preview: known limitations

Current preview: **0.9.12**.

- **Windows 11 x64 only.** Windows 10 and native ARM64 support have not been established.
- **Unsigned portable executable.** No signed installer is included. Windows or security software may warn or block it.
- **Independent clean-machine verification is pending.** Development checks include native UI and file-operation tests, but a separate fresh Windows installation has not yet been verified for this public package.
- **Use replaceable copies while testing.** Power loss, process termination, disconnected drives and concurrent changes need broader real-world validation. Copying is not a transactional backup and does not verify destination content hashes automatically.
- **Undo is session-limited.** Eligible operations are retained for the current session, within bounded history. Permanent deletion, replaced files, other apps' actions and past sessions are not generally recoverable through Ximple's undo.
- **Search is by filename and metadata.** There is no file-content search or permanent whole-disk index. Capped, incomplete and provisional results are labelled in the app.
- **ZIP browsing has limits.** Archive members cannot be renamed or edited in place. Some archive formats and encrypted archives are unsupported; extraction is separate from ordinary folder editing.
- **Cloud and network behavior varies by provider.** Thumbnail and individual-icon loading is restricted for certain cloud/network/offline items to avoid fetching file contents just for display. Broader provider testing is still needed.
- **Space scans are snapshots.** Results can become outdated after other applications change files. Partial totals and scan limits are labelled; file links can be skipped.
- **Security integrations are not safety guarantees.** Defender scans and VirusTotal report links require their respective Windows/service capabilities. An existing VirusTotal report is not a new scan. Ximple does not automatically upload files to VirusTotal.
- **Accessibility and unusual display configurations need more testing.** Feedback from keyboard, screen-reader and high-scaling users is welcome.
- **Purchase and activation are not connected.** The preview is unlocked and has no automatic expiry. Final-version pricing and release timing are undecided.

Please [report specific failures](https://github.com/KaalBrown/ximple-explorer/issues/new?template=bug-report.yml), including the version and steps needed to reproduce them.
