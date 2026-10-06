# SHANEX Print Manager V6.0.0 Native

> Draft release notes for tag `V6`.

SHANEX Print Manager V6 is the major native-generation release. It moves the product forward with the new Windows-native desktop stack, a rebuilt self-service kiosk experience, stronger pricing/costing workflows, upgraded Quick Look, improved WhatsApp verification, tenant branding, receipt artwork options, and a new native installer pipeline.

## Highlights

### Native V6 platform
- Native Windows desktop generation based on WPF/.NET 10.
- Native-AOT ShanexCore engine packaged with the desktop application.
- Native WhatsApp sidecar integration and shared native product versioning.
- Product, assembly and file version aligned to **6.0.0**.

### Self-Service Kiosk
- Reworked kiosk experience with cleaner responsive UI, motion, progress feedback and customer-friendly flows.
- Added desktop WhatsApp verification using a QR code and mobile verification using a WhatsApp deep link.
- Added Quick Print flow with live quantity-tier savings feedback.
- Added clear print-progress stages so customers can see what the system is actually doing.
- Added shop-branded idle/attract experience.
- Added Public Documents browsing/printing experience.
- Added Sinhala and Arabic runtime coverage for public-library flows.
- Improved customer help flow so staff-help requests are separated from payment approvals.

### Kiosk Admin & security
- Added dedicated kiosk admin web controls.
- Added LAN-only admin credential provisioning.
- Added persistent manual kiosk-admin password and recovery controls.
- Manual passwords use a salted PBKDF2 verifier rather than storing the password itself.
- Successful password change/reset revokes active admin sessions.
- Public deployment checks are designed to keep `/admin` and `/api/admin/*` unavailable through the public Cloudflare path.

### Shop branding
- Kiosk branding now follows the existing Interface & Identity settings.
- Custom shop name and logo can be pushed into the kiosk automatically.
- Removed customer-facing SHANEX hard-coding from tenant kiosk surfaces where shop branding should be authoritative.
- Added live branding refresh and tenant-safe fallback copy.

### Pricing & Materials
- Reworked the native **Prices & Costing** workspace.
- Improved Customer Price List editing, search, add/edit/duplicate and advanced bulk-pricing flows.
- Separate Paper, Machine and Finishing profile editors.
- Added archive/restore workflows for production profiles.
- Added guards around default Paper and Machine profiles.
- Improved installed-printer mapping and warnings for missing saved mappings.
- Added a clearer Price Calculator using the same canonical costing engine as production jobs.
- Preserved historical costing snapshots and existing quotation/reporting boundaries.

### Kiosk pricing
- Added stricter kiosk pricing configuration with live refresh.
- Invalid public-kiosk pricing fails closed instead of silently using guessed/stale values.
- Added quantity-tier savings calculation and customer-facing savings display.

### Quick Look
- Fixed grid layout so PDF page tiles wrap correctly inside the viewport.
- Fixed thumbnail sidebar scrolling.
- Thumbnail click now scrolls/focuses the matching page reliably.
- Added scroll-driven lazy page rendering and active-page tracking.
- Added **Ctrl + mouse wheel** zoom with bounded zoom levels.
- Added switchable side and classic horizontal thumbnail layouts.
- Added persistent thumbnail-orientation preference.
- Restored animated grid-tile hover behavior.
- Added regression coverage for 1-page, 55-page and 500-page documents.

### Receipts & customer artwork
- Added optional customer profile picture support for receipt artwork.
- Customer avatar use is privacy-first and defaults to **OFF**.
- Added optional shop logo/customer thumbnail support across PDF, thermal/custom-template and WhatsApp receipt artwork.
- Receipt artwork decorates authoritative receipt data without changing monetary calculations.
- Missing or unavailable optional artwork falls back safely to the normal text/vector layout.

### Installer & packaging
- New native WiX installer pipeline for V6.
- Packages the x64 Desktop, Native-AOT ShanexCore, PrintTicket helper, WhatsApp sidecar and approved Ghostscript runtime.
- Improved Ghostscript discovery from explicit path, environment variable, repo-local runtime, PATH or Program Files.
- Added payload/version validation before packaging.
- Added kiosk asset validation to prevent incomplete installers.
- Added same-version major-upgrade behavior for V6 support builds.
- Installer build emits SHA-256 hashes for MSI/setup outputs.
- Final setup output: `native-next/dist/SHANEX-Print-Manager-Setup.exe`.

### Reliability & engineering
- Fixed native drawing/image type build regressions.
- Added/expanded native Release validation scripts and focused regression coverage.
- Added release-package metadata validation.
- Improved kiosk release, upgrade and rollback documentation.

## Important draft-release note

This V6 entry is intentionally a **draft**. Source/package structure is prepared, but final public release should only be published after the Windows Release validation, installer install/upgrade checks, clean-machine verification and real-device/printer/payment acceptance are completed.

---
SHANEX Print Manager V6.0.0 Native
