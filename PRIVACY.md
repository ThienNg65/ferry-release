# Privacy Policy for Ferry

**Effective Date:** 2026-11-23  
**Policy Version:** 1.1  
**Maintainer / Data Controller:** ThienNg65  
**Contact:** [GitHub Issues on ThienNg65/ferry-release](https://github.com/ThienNg65/ferry-release/issues) · [ferryssh.com/privacy](https://www.ferryssh.com/privacy)

Ferry is a free, local-first Windows desktop SFTP and SSH client. The desktop app operates with zero telemetry, zero accounts, and zero analytics. Historical source releases were distributed under the MIT License (see [LICENSE](LICENSE)); downloading a packaged installer does not change rights already granted to earlier source releases.

## 1. Ferry Desktop App — Data We Do Not Collect

The Ferry desktop app does **not**:
- Collect, transmit, or sell personal data, usage telemetry, crash reports, or behavioral analytics.
- Use HTTP cookies, advertising identifiers, or third-party tracking SDKs. (The application UI enforces a strict `default-src 'self'` Content Security Policy.)
- Require user accounts, collect email addresses, or send marketing communications.
- Process payments, subscriptions, or financial information.
- Use AI models or send any user data or files for AI training.
- Knowingly collect personal information from anyone, including children under 13 (or the applicable age of digital consent).

## 2. Data Stored Locally on Your Device

All Ferry desktop configuration and state is stored **exclusively on your local Windows machine** under your OS user data directory (`%APPDATA%\Ferry`) and WebView `localStorage`:

| Data | Storage Location | Purpose | Protection |
|---|---|---|---|
| Saved Sites & Proxy Settings | `sites.json`, `app-settings.json` | Store hostnames, ports, usernames, key paths, and preferences | Passwords and key passphrases are encrypted at rest using Windows DPAPI (`CryptProtectData`) and never leave the local backend process decrypted |
| Transfer & Operation History | `history.json` | Show recent transfers/operations in History | Capped at 2,000 entries and subject to your configured retention limit (default: 90 days) |
| Trusted SSH Host Keys | `known_hosts.json` | Trust-on-first-use SSH host-key verification | Local SHA-256 fingerprints; manageable/deletable in Settings |
| Directory Bookmarks | `bookmarks.json` | Quick navigation to saved folders | Local JSON |
| UI & Window Preferences | WebView `localStorage` | Theme, accent color, column layout, pane width, window bounds | Local browser storage only |
| Runtime Diagnostic Log | `neutralinojs.log` | Local Neutralino shell diagnostics | Written locally only |
| Temporary Staging / Edit Files | OS temp directory | Staging OS drag-and-drop uploads and external file edits | Cleaned up after transfer or edit session close |

## 3. Network Connections

The Ferry desktop app only initiates outbound network connections in two situations:
1. **Your SSH / SFTP / Proxy Connections:** When you connect to a server, Ferry connects directly to the hostnames, jump hosts, or proxies you configure.
2. **Application Update Checks (Optional):** When **Automatically check for updates** is enabled (or when you click **Check for updates**), Ferry fetches `latest.yml` and verified release installers from `https://github.com/ThienNg65/ferry-release/releases/latest/download`. GitHub's standard server logs and [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement) apply to that HTTP request. You can disable automatic update checks at any time in **Settings → Updates & About**.

## 4. Data Retention, Access & Deletion

Because all desktop configuration is stored locally on your device, you have direct control at all times:
- **Retention Limits:** In **Settings → Privacy & Legal**, you can set the transfer/operation history retention window (`30 days`, `90 days`, `1 year`, or `Unlimited`). Expired entries are pruned automatically.
- **Data Access (Export):** Use **Settings → Privacy & Legal → Export My Data** to export a JSON file containing your local settings, site metadata (excluding passwords/passphrases), bookmarks, known hosts, and history.
- **Data Deletion:** Use **Settings → Privacy & Legal → Delete All Local Data** to permanently erase all saved sites, encrypted credentials, bookmarks, history, known hosts, settings, and UI preferences, or manually delete `%APPDATA%\Ferry`.

## 5. Website Analytics (`ferryssh.com`)

Unlike the Ferry desktop app, the `ferryssh.com` marketing website uses privacy-friendly, cookie-free **Vercel Web Analytics** to measure aggregate page views and outbound download/Microsoft Store clicks. It does not set cookies, store personal identifiers, or track visitors across other websites.

## 6. Changes to This Policy

Updates to this Privacy Policy will be published in `PRIVACY.md` and on [ferryssh.com/privacy](https://www.ferryssh.com/privacy) with a new Policy Version and Effective Date. Material changes will re-prompt acceptance in the application.
