# CHANGELOG - Alsyundawy Professional System Administrator Portfolio

All notable changes to this project are documented in this file in accordance with [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and [Semantic Versioning](https://semver.org/).

---

## [8.5.5] - 2026-10-06

### Added & Expanded (Repositories & Tools)

- **Showcase Expansion (Total 40 Repositories)**:
  - **PowerDNS-Admin-PHP** (`https://github.com/alsyundawy/PowerDNS-Admin-PHP`): Enterprise Authoritative PowerDNS Web Control Plane in Native PHP & PDO without external frameworks. Sub-millisecond bootstrap (<1ms), zero-CDN offline capability, RFC 6238 TOTP 2FA authentication, multi-server node clustering, APCu caching, and PowerDNS HTTP API v1 integration.
  - **SubnetCalc-MacOS** (`https://github.com/alsyundawy/SubnetCalc-MacOS`): High-performance native Swift & AppKit Cocoa IPv4/IPv6 subnet calculator for macOS Universal 2 (Apple Silicon M1-M4 & Intel x64). Equipped with 25 developer theme suites, CIDR/VLSM calculation, netmask, wildcard mask, and hierarchical menu navigation.
  - **SubNetCalc-Electron** (`https://github.com/alsyundawy/SubNetCalc-Electron`): High-precision, memory-efficient IPv4/IPv6 subnet calculator for macOS & cross-platform desktop. Built with Electron 44, Node 24, React 19, and TypeScript; features 14 multi-themes, RFC classification, binary bit visualization, and real-time CIDR computation.

### Fixed & Hardened (13-Pillar Code Quality & Security)

- **Bug 1 (Cryptographic Nonce Fallback)**: Hardened CSP nonce generation fallback logic in `index-portofolio-8.5.5.php`. Hardened CSP nonce fallback using cryptographic `openssl_random_pseudo_bytes(16, $is_strong)` with deep SHA-256 entropy fallback; eliminated weak hash (`md5`) and weak PRNG (`mt_rand`), fully satisfying SonarLint rules S4790 & S2245.
- **Bug 2 (Psalm Strict Comparison)**: Resolved Psalm `RiskyTruthyFalsyComparison` on `$_SERVER['HTTPS']`. Enforced strict check `isset($_SERVER['HTTPS']) && $_SERVER['HTTPS'] !== '' && $_SERVER['HTTPS'] !== 'off'`.
- **Bug 3 (404 Resource Elimination)**: Converted absolute root asset references (`/favicon.svg`, `/favicon.ico`, `/sitemap.xml`) to portable relative paths (`favicon.svg`, `favicon.ico`, `sitemap.xml`), completely eliminating 404 console errors in file environments and subpaths.
- **Bug 4 (SonarLint Code Smell)**: Centralized duplicated string literals into global constants (`ICON_SERVER`, `ICON_SHIELD`, `ICON_NETWORK`, `ICON_APPLE`).
- **Bug 5 (SEO Freshness)**: Updated Schema.org structured data `dateModified` to `2026-10-06T00:00:00+07:00`.
- **Bug 6 (HTML/ARIA Standards)**: Removed redundant `role="navigation"` on `<nav>` and redundant `role="main"` on `<main>`; added explicit `type="button"` on back-to-top button; optimized title length to under 70 characters.

### Responsive & Viewport Hardening (Xiaomi Redmi, POCO & Universal)

- **Viewport Fit Cover**: Added `viewport-fit=cover` to `<meta name="viewport">` for edge-to-edge rendering and notch/cutout containment on Xiaomi Redmi, POCO, and iPhone devices.
- **Android Text Inflation Suppression**: Added `-webkit-text-size-adjust: 100%`, `-moz-text-size-adjust: 100%`, and `text-size-adjust: 100%` on `html` to prevent Android Chrome / MIUI / HyperOS font boosting from inflating text and causing container clipping.
- **Hardware Safe-Area Insets**: Applied `env(safe-area-inset-*)` padding on `.navbar`, `.footer`, `.back-to-top`, and `body`.
- **Text & Grid Overflow Protection**: Enforced `overflow-wrap: anywhere` and `min-width: 0` on all cards and titles, preventing unhyphenated repository names from expanding grids past the screen boundary.
- **Mobile Navbar Scrolling Guard**: Added `max-height: 80dvh; overflow-y: auto;` to `.navbar-collapse` on small mobile viewports.
- **Multi-Device Automated Playwright Suite**: Verified 100% passing across 20 distinct device viewports and screen densities (VGA 640x480 up to 2K 2560x1440 and 4K) with 0px horizontal overflow and zero console errors.

### Linter & Toolchain Clearance

- `phpcs --standard=PSR12`: 0 errors, 0 warnings.
- `phpstan analyse --level=max`: 0 errors.
- `psalm --no-cache`: 0 errors, 0 warnings, 0 info issues.
- `php -l`: Syntax check 100% OK.
- `php-cs-fixer`: @PSR12 compliance verified.
- `eslint`: Flat config valid, zero warnings.
- `stylelint`: Embedded CSS rules clean, zero warnings.
- `prettier`: Formatting clean.

---

## [8.5.4] - 2026-09-23

### Added in v8.5.4

- Integrated 4 showcase repositories (total 37): `pear-desktop-mac`, `PnetLab-v8`, `Disable-MacOS-Updates`, `openssl-1.0.2`.
- Added PNETLab deployment tutorials and documentation.

---

## [8.5.3] - 2026-09-21

### Added in v8.5.3

- Integrated 3 showcase repositories (total 33): `PHP-PDNSManager`, `bailu-kilo-agent`, `PHP-BindManager`.
- Added `Visual Subnet Calculator` to tools suite (total 13).
