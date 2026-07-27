# SHANEX Print Manager Pro v4.1.2

Release date: 27 July 2026

This release focuses on print-production tools, licensing reliability, WhatsApp stability, portable configuration, POS clarity, and general workflow improvements.

## Highlights

- Added portable full and selective settings transfer between SHANEX installations.
- Added advanced global and per-printer X/Y print-position calibration.
- Added business-card, bill-book and sticker imposition improvements.
- Upgraded online licensing to signed v3 entitlement and lease tokens.
- Improved WhatsApp contact, media and international-number handling.
- Improved POS payment history and print/product grouping.

## Printing and imposition

- Added last-used settings restoration and reusable imposition presets.
- Added automatic source-document size and PDF bleed detection, with manual overrides.
- Added source-document and export-document summaries.
- Added configurable cut-mark length and distance from artwork.
- Added a clean cut-mark mode that avoids unnecessary marks inside artwork.
- Fixed the imposition preview layout so the preview remains visible on the right.
- Added separate artwork and output-sheet previews for numbering workflows.
- Added settings reset controls.
- Fixed incomplete sheet filling and damaged PDF exports in sticker imposition.
- Added an option to rotate the lower bill-book row by 180 degrees for outward-facing binding edges.
- Added sticker numbering with configurable start number, padding, prefix, suffix, font, size, position and colour.
- Added optional hidden `CutContour` output for plotter and die-cut workflows.
- Added configurable rounded sticker corners.
- Added Crash Numbering Gothic and Crash Numbering Serif support.
- Expanded the B/W sketch filter range with progressively darker strength levels.

## Print defaults and calibration

- Added `Settings â†’ Printing Defaults â†’ Advanced Print Settings`.
- Moved user-facing X/Y calibration controls out of Developer Settings.
- Added global X and Y offsets.
- Added independent per-printer X and Y offsets.
- Added alignment reset and calibration guidance.
- Preserved compatibility with existing saved offset values.

## Settings transfer

- Added portable JSON export and import under `Settings â†’ System & Backup`.
- Added full portable settings export.
- Added selective export/import for:
  - Price lists and paper types
  - Products and variants
  - Print defaults and X/Y alignment
  - Print-setting templates
  - Shortcuts and template keys
- Selective import changes only the categories contained in the file.
- Machine-specific paths, licence data and saved account passwords are excluded from portable backups.

## WhatsApp

- Improved contact synchronization reliability.
- Improved normalization and handling of international phone numbers.
- Improved media download and missing-file recovery behavior.
- Improved date-folder rollover for applications left running across multiple days.
- Improved startup recovery and persisted-log handling.
- Improved duplicate-file and stale-preview handling.

## POS, payments and file status

- Products are now displayed with print files according to the date they were added.
- Added clearer date separators and completed-print indicators.
- Print items and product items paid together are now stored as a single payment group.
- Payments can be taken before printing is completed.
- Added paid-state records and warnings when attempting to charge an already-paid item.
- Improved visual setting indicators and replaced Unicode status symbols with SVG icons.
- Improved deleted-file detection to reduce false â€œfile deletedâ€ states.
- Fixed unwanted automatic chat scrolling while reviewing older messages.
- Improved print-processing progress feedback.

## Licensing and telemetry

- Added signed v3 entitlement and lease-token support.
- Added automatic legacy-licence upgrade to v3 leases.
- Added remote hardware-ID block checks before lease renewal.
- Added safe recovery after an administrator removes a hardware block.
- Added D1 entitlement, lease, trial-extension, emergency-unlock and server-worker schemas.
- Removed a path that could allow a client ingest credential to add hardware IDs to the block list.
- Fixed duplicate licence API routes and malformed telemetry D1 writes.
- Added strict machine-ID validation.
- Added separate admin and ingest authentication paths.
- Added Sri Lanka time display for application logs and telemetry dashboards while retaining UTC storage.

## Installer

- Improved the uninstall licence-removal confirmation.
- Added bilingual Sinhala and English guidance.
- Licence deletion now defaults to `No` to reduce accidental removal.
- Temporary cache cleanup is separated from licence-data removal.
- Customer databases, sales data, print history and business records remain preserved.

## Fixes and maintenance

- Fixed missing C# dispatcher mappings for licence upgrade, server-token storage, revocation and network diagnostics.
- Fixed stale licence-gate cache after token renewal or server revocation.
- Fixed duplicate startup licence refresh behavior.
- Improved startup diagnostics and error reporting.
- Added safer D1 indexes for entitlement and lease lookups.
- Updated Cloudflare Worker configuration and production deployment checks.

## Upgrade notes

- Back up the local database before upgrading.
- Existing print presets, price lists and printer offsets remain compatible.
- Restart SHANEX after importing printer, interface or WhatsApp settings.
- A valid signed v3 lease is required to clear a server-revoked state after an administrator unblocks a machine.


➡️ **[Download the latest release](https://github.com/shashmithx/shanex-print-manager-releases/releases/latest)**

See [all releases](https://github.com/shashmithx/shanex-print-manager-releases/releases) for previous versions.

---
© 2024–2026 SHANEX.LK · Developed by Shashmith Ayoddaya
