# Data and network behavior

This describes the **0.9.12 development preview**, not a promise about unimplemented future services.

- No application telemetry or automatic crash-report submission is implemented.
- Settings are stored locally under `%LOCALAPPDATA%\XimpleExplorer`. They can include folder paths, tabs, pins, color labels and preferences. Scan history stores folder paths and totals locally.
- Browsing network shares and cloud-provider folders, or opening files in another app, may cause Windows, the provider or that app to access the network.
- Microsoft Defender scanning invokes the installed Windows capability. Defender and Windows Security have their own behavior and settings.
- VirusTotal lookup calculates a SHA-256 fingerprint locally. Opening a report sends that fingerprint to VirusTotal through your browser. Folder lookup prepares fingerprints locally; report links are opened when selected.
- Ximple does not automatically upload files to VirusTotal. Choosing a manual upload on its website, including dropping a file onto that site, sends the file through the browser.
- Opening website links uses your browser. GitHub hosts these downloads and public reports under its own terms and privacy policy.
- Public bug reports and community comments are public. Remove personal information and secrets before posting. Ximple does not require you to submit personal files to report a problem.

Checkout, license activation and update-service policies will need to be described before those services are implemented. They are not connected in this preview.
