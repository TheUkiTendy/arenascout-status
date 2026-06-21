# Security Policy

## Trust posture

ArenaScout is a **local-first** desktop app: it reads your local MTG: Arena `Player.log` and stores
everything (matches, decks, stats, opponent names) in a database **on your own machine**. It has no
account or login and does not upload your match data. The only things that can leave your device are
the few, mostly-optional network features documented in **[PRIVACY.md](./PRIVACY.md)**.

Because the app isn't code-signed yet, Windows SmartScreen may warn on first run. That's expected for
an unsigned indie app — see the [README](./README.md#windows-protected-your-pc--is-this-safe) for why,
and for how to install safely.

## Verifying a release

Every release ships with two free, independent integrity signals:

- **SHA-256 checksum** — a `SHA256SUMS.txt` asset plus the hash in the release notes. Confirm your
  download before running:

  ```powershell
  Get-FileHash "$HOME\Downloads\ArenaScout Setup <version>.exe" -Algorithm SHA256
  ```

- **VirusTotal report** — a link in the release notes to a scan of the exact installer by ~70
  antivirus engines. You can re-upload your own copy to double-check.

If a checksum doesn't match, **do not run the installer** — re-download from the official
[Releases page](https://github.com/TheUkiTendy/arenascout-status/releases).

## Reporting a vulnerability

Please report security issues by **opening an issue** on this repository
(<https://github.com/TheUkiTendy/arenascout-status/issues>). Don't include sensitive details in a
public issue — just say you've found a security concern and we'll arrange a private channel to follow
up. We aim to acknowledge reports promptly and fix verified issues in a timely release.

## Supported versions

ArenaScout is pre-1.0 and ships frequently; security fixes land in the **latest** release. Always run
the newest version from the [Releases page](https://github.com/TheUkiTendy/arenascout-status/releases).
