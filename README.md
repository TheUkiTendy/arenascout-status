# ArenaScout

**ArenaScout** is a local match tracker for *MTG: Arena*. It reads the `Player.log` file the Arena
client already writes to your PC, records your matches, builds opponent profiles, and surfaces stats
the Arena client doesn't expose. **Your data stays on your machine** — there's no account, no login,
and your match history, decks, and opponents are never uploaded.

This public repository hosts ArenaScout's **release installers**, its **privacy & security docs**, and
the small `status.json` the app reads for update/service notices.

➡️ **[Download the latest release](https://github.com/TheUkiTendy/arenascout-status/releases/latest)**

---

## "Windows protected your PC" — is this safe?

When you run the installer you may see:

> **Windows protected your PC** — Microsoft Defender SmartScreen prevented an unrecognized app from
> starting.

**This is expected, and the app is not malware.** SmartScreen shows this for *any* program that
isn't signed with a (paid) code-signing certificate **and** hasn't yet been downloaded by enough
people to build "reputation." ArenaScout is a free, hobby app made by one developer, so it hasn't
bought a certificate yet. The warning is a caution prompt — **not a block**.

Microsoft changed this in March 2024: a certificate no longer removes the prompt instantly, so
reputation now has to build up through downloads over time. As more people install ArenaScout, the
warning will fade on its own.

### How to install anyway

1. On the blue SmartScreen dialog, click **More info**.
2. Click **Run anyway**.
3. Continue through the installer.

### Verify the download yourself (recommended)

Don't just take our word for it — every release lets you check the file independently:

- **Checksum.** Each release includes a `SHA256SUMS.txt` and lists the SHA-256 hash in the release
  notes. Confirm your download matches before running:

  ```powershell
  Get-FileHash "$HOME\Downloads\ArenaScout Setup <version>.exe" -Algorithm SHA256
  ```
  The printed hash should equal the one in the release notes. If it doesn't, **don't run it** — the
  file was corrupted or tampered with in transit; re-download.

- **VirusTotal.** Each release links a [VirusTotal](https://www.virustotal.com) report, where ~70
  antivirus engines scan the exact installer. You can also upload your own copy there to double-check.

---

## What data leaves your PC

ArenaScout is built local-first. The full policy is in **[PRIVACY.md](./PRIVACY.md)** (and inside the
app under *Privacy*), but in short — the only things that can ever leave your device are:

| Feature | When | What's sent | Identifier? |
|---|---|---|---|
| **Card detail lookups** | On by default (you can turn it off) | Only a numeric **card ID** for cards too new to be bundled, to [Scryfall](https://scryfall.com) | No |
| **Update / service check** | Packaged app, periodic | Nothing about you — fetches one **public** file from GitHub | No |
| **Anonymous diagnostics** | On by default (you can turn it off) | App version + basic device info (e.g. OS) | **No identifier** |
| **Optional usage stats** | **Off** unless you opt in | Adds a random install id + a count of recorded matches | Random install id only |
| **Feedback** | Only if you use it | Saved as a **local file**; nothing is auto-uploaded | — |

**Never sent:** your Arena login or password, your real name, the contents of your matches or chats,
your decklists, or the identities of your opponents. Opponent names are shown to *you* locally so you
can review your own games — they are never uploaded.

---

## Reporting a problem

For privacy/data requests or to report a security issue, see **[SECURITY.md](./SECURITY.md)** or open
an issue on this repository. Please don't include sensitive personal details in a public issue.

---

<sub>This repo also hosts `status.json`, the small public manifest the app reads for update and
service notices.</sub>
