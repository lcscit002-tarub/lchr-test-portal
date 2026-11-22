# LC Employee Portal v2.10 – Bilingual Login Help Text

This is a static, design-first prototype for the Luo City Spa Club Employee, Manager, and HR portals. Supabase is intentionally not connected.

## Run locally

Open `index.html` in a modern browser. For best results, serve this folder with a simple static server or deploy it to Cloudflare Pages.

## Demo access

- Employee: ID `758` / Password `demo123`
- Manager: ID `MGR-01` / Password `demo123`
- HR: ID `HR-ADMIN` / Password `demo123`

The role-specific Demo button can also enter the selected demo portal.

## v2.4 refinements

- Lowered the welcome logo and text toward the role modal.
- Added a subtle shadow to the logo and welcome text.
- Added 1px letter spacing and a subtle shadow to the role modal heading.
- Set Employee / Manager / HR buttons to the `CY Grotesk V3 Wide` font family with Garet Heavy fallback. **The supplied package did not include the CY Grotesk V3 Wide font file.** To guarantee the exact typeface across all devices, add a licensed `.woff2`, `.woff`, or `.ttf` file to `assets/fonts/` and define it with `@font-face` in `styles.css`.
- Standardized the portal header date and time to Telegrafico with matching size and weight.

## Deployment to Cloudflare Pages

Upload the extracted contents of this folder to the root of a GitHub repository. In Cloudflare Pages use:

- Framework preset: None
- Build command: leave blank
- Build output directory: `.`
- Root directory: leave blank

## Important

This package is a local demo only. It uses browser-local demo state and does not provide production authentication, shared database storage, payroll processing, or multi-device synchronization. Do not enter real employee personal information or payslips.


## v2.5 font corrections

- Bundled the supplied **CY Grotesk Wide Medium** font and applied it to Employee / Manager / HR role buttons using its native Medium weight.
- Normalized the full date-and-time line (footer and signed-in header) to Garet Heavy so letters, digits, and punctuation render in one consistent font.
- The supplied `Telegrafico.ttf` has alphabetic glyphs but does not include numerical glyphs; the browser was therefore mixing Telegrafico letters with fallback numerals. Garet Heavy is used for the entire date/time string to eliminate the visible mismatch.

### Font licence notice
The README supplied inside the CY Grotesk download states **personal use only** and says commercial use and redistribution are not allowed. This package includes the supplied font only for local design preview. Do not push this font file to a public GitHub repository or deploy it for company/commercial use unless you obtain the appropriate commercial licence or written permission. Replace it with a properly licensed font file before production deployment.


## v2.6 visual adjustments

- Moved the LCSC logo and welcome wordmark lower, closer to the role-selection card.
- Removed the drop shadow from the logo image; retained a subtle shadow on the welcome text only.
- Increased the welcome wordmark from 15.6px to 20.6px.
- Replaced the role-button font with the latest user-supplied CY Grotesk Wide font file.
- Applied that same CY Grotesk Wide face to the complete date/time strings in the welcome footer and signed-in header, preventing mixed fallback glyphs.
- Updated CSS/JS query versions to 2.6.0 to avoid serving stale cached resources.

### Font licence reminder
The README included in the user-supplied CY Grotesk Wide archive states personal, non-commercial use only. This font is included for the local design-preview package. Obtain a suitable commercial licence or written permission before publishing it in a company GitHub repository or deploying it for business use.


## v2.6 visual revision (22 November 2026)

- Moved the logo and LCSC welcome wordmark closer to the role-selection modal.
- Removed shadow from the logo image; retained a subtle shadow on the text only.
- Increased the wordmark to 20.6px (responsive sizes apply on smaller screens).
- Replaced the Employee/Manager/HR role-button font with the newly supplied CY Grotesk Wide TTF.
- Applied that same CY Grotesk Wide font face to the complete welcome footer and signed-in portal date/time displays.
- Bumped CSS/JS query versions to v2.6.0 and used a fresh font filename to avoid stale cached assets.

### Font licence reminder
The README included inside the user-supplied CY Grotesk Wide archive states that the download is for personal, non-commercial use only and that commercial use and editing for redistribution are not permitted. This font is bundled for local design preview only. Obtain the appropriate commercial licence or written permission before publishing it to a company GitHub repository or deploying it for business use.


## v2.7 welcome spacing refinement

- Changed the welcome screen to a single responsive vertical flex group containing the LCSC logo/wordmark and role-selection card.
- Set the gap between the brand block and role-selection card to exactly 35px at all viewport sizes.
- Removed independent percentage-based top positioning from the welcome brand, which caused different apparent spacing across monitors.
- Kept the existing logo, fonts, colors, role-selection card, modal behavior, and login flow unchanged.
- Added vertical scrolling for unusually short viewports rather than allowing the brand and modal to overlap.
- Updated stylesheet and JavaScript cache query versions to 2.7.0.


## v2.9 login help-text sizing correction

- The login-page forgot-password instruction now uses the same responsive Garet Book typography as the first-page role-selection note.
- At narrow/mobile viewport widths, both resolve to `clamp(7.5px, 2.35vw, 10.5px)`; at wider viewports, both use `clamp(9px, 1vw, 11.5px)`.
- Both use regular weight and 1.25 line-height. The longer login message remains allowed to wrap naturally so it does not overflow the login card.
- Updated asset query versions to `2.9.0` to reduce stale stylesheet/script reuse.


## v2.10 update

- The forgot-password English message and Chinese translation now appear on separate centered lines.
- The vertical separator character has been removed.
- Existing typeface, responsive font size, line-height, colors, and login behavior are preserved.
