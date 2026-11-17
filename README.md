Mahwar V2.1 Encrypted Backups — purpose and privacy notice
Updated 17 November 2026

This private operational tool creates encrypted disaster-recovery backups for Mahwar HR. It is operated by the Mahwar account owner. It is not an application for general public use.

Google Drive access is limited to drive.file: files created by this tool or explicitly selected for it. The tool checks the authorized account identity and the backup folder's location and access permissions. It uploads four encrypted backup files per run, then downloads those encrypted files to verify their size and SHA-256 fingerprints. The approved backup folder and files remain restricted to their owner.

Database backup content is encrypted before upload. The decryption identity is not uploaded to Google Drive or stored in GitHub Actions. The hosted runner temporarily processes backup data in memory; the backup workflow publishes metadata receipts only, without plaintext database content or authentication secrets.

Google Drive stores the encrypted backup files in the owner's account. GitHub Actions runs the private backup workflow and stores its restricted credentials as encrypted repository secrets. Backups are retained for at least 30 days; the workflow does not delete them. The owner can revoke the tool's Google access from Google Account security settings and manage retained files directly in Drive.

Google user data is used only for backup storage, integrity verification and access checks. It is not sold, used for advertising, or used to develop, improve or train AI or machine-learning models. This notice contains no employee records, backup locations, credentials or decryption keys.

Questions or requests: contact the Mahwar account owner through the support email displayed on the Google OAuth consent screen.
