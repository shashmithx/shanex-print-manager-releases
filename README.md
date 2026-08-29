# SHANEX Print Manager v5.0.4

SHANEX Print Manager Pro is a print-shop workflow platform for customer jobs, PDF printing, POS, scanning, printer monitoring, WhatsApp-assisted workflows, and multi-PC shop operations.

## What's New in v5.0.4

Version 5.0.4 focuses on stability, printer monitoring, live copier workflows, server-mode groundwork, and UI refinement.

### Server Mode & Multi-PC Workflow

- Expanded the Server Mode foundation for shared shop workflows and central operation.
- Improved center-panel behavior and related UI states for server-oriented workflows.
- Hid kiosk-specific settings automatically when kiosk mode is disabled.

### Printer Monitoring & Photocopy Counter

- Fixed and hardened SNMP polling used for printer and copier monitoring.
- Added a live photocopy auto-counter workflow.
- Added live counter UI updates and improved synchronization between copier data and the interface.

### Printing & Receipts

- Improved thermal receipt output so important text prints with stronger visibility and contrast.
- Added safer handling for receipt template markup and thermal output generation.
- Improved printing behavior related to light or low-contrast output.

### Reliability & Internal Communication

- Fixed Native AOT pipe response serialization used by native/helper components.
- Strengthened duplicate file-import suppression to prevent the same incoming file from being added repeatedly.
- Improved live UI state synchronization around photocopy monitoring.

### Interface Improvements

- Refined the center panel and general application UI.
- Improved visibility and state handling for settings that only apply to specific operating modes.

---

## SHANEX V5 Highlights

### Modern Interface

- Added optional SHANEX V4 Classic, SHANEX V5, SHANEX macOS Dark, and SHANEX macOS Light themes.
- Theme selection is saved locally and restored automatically after restart.
- Improved responsive Center Panel toolbars to prevent overlapping controls on smaller screens.
- Improved customer cards, spacing, controls, profile-picture display, and phone-number readability.
- Customer phone-number size can be adjusted from Settings and applies across supported themes.

### Print Queue and File Workflow

- Click anywhere on a file row to select it, except on interactive controls such as inputs, checkboxes, buttons, and drag handles.
- Product rows can be selected directly from the queue.
- Improved queue spacing, selected states, date grouping, and file-row readability.
- Improved print template capture and application for printer, tray, paper, media type, print quality, duplex, colour mode, N-up, booklet, and page-selection settings.
- Improved printer capability loading and printer setting refresh behavior.
- Added safer handling for stale per-file print settings.

### Printing and PDF Reliability

- Improved native PDF print routing and vector-print reliability.
- Improved handling for fillable PDF forms before printing.
- Improved Quick Look support for Sinhala fonts, Unicode file paths, page operations, cropping, rotation, and restoration.
- Improved preview loading behavior for scanned and image-heavy documents.
- Improved paper size, tray, media type, duplex, and printer quality handling.
- Added stronger function-key print-template support.

### Scanner Integration

- Added NAPS2 scanner integration.
- Added configurable scanner presets, DPI, colour mode, page size, output type, and scanner selection.
- Added scan-to-PDF and scan-to-image workflows.
- Added scan preset keyboard shortcuts.
- Added alternating-page rotation support for scanning workflows.

### Image Studio and Imposition Tools

- Improved Image Studio controls, layout tools, crop marks, boundaries, PDF import, and output setup.
- Improved Imposition Tools for business cards, bill numbering, cut marks, carbon-copy planning, and print-ready layouts.
- Added improved planning previews and custom layout controls.

### POS and Payments

- Improved Product Checkout workflow and keyboard navigation.
- Improved product selection, quantity editing, cart navigation, and customer-queue integration.
- Added improved product/service handling alongside print jobs.
- Improved payment, outstanding balance, credit, receipt, and Ready-for-Pickup workflows.

### WhatsApp and Customer Workflow

- Improved WhatsApp startup recovery and media reconciliation.
- Improved customer profile-picture loading and caching.
- Improved Ready-for-Pickup, payment receipt, and customer message workflows.
- Improved customer search, recent-customer access, and queue navigation.

### Printer Monitoring and Reports

- Added Printer Monitor and monitoring improvements.
- Improved printer counter, fault, status, and monitoring workflows.
- Added better daily reporting and worker activity reporting support.
- Improved printer capability detection and machine configuration handling.

### Performance and Reliability

- Reduced unnecessary preview and media processing.
- Improved file metadata indexing and queue loading behavior.
- Improved startup recovery and dependency handling.
- Improved automatic update reliability.
- Improved customer-data safety during upgrades and recovery operations.
- General stability, usability, and performance improvements throughout the application.

## Upgrade Notes

- Existing customer data, print settings, and templates are preserved during standard upgrades.
- Existing themes remain available.
- No manual migration is required for standard local installations.

See [CHANGELOG.md](CHANGELOG.md) for version-by-version changes.
