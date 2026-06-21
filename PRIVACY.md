# ArenaScout — Privacy Policy

ArenaScout is built to keep your data on your own machine. This policy explains what stays local, the
few things that can leave your device, why, and the choices you have.

## The short version

ArenaScout runs locally and reads the log your MTG: Arena client already writes to your computer.
Your match history, decks, statistics, and the names of opponents you have played are stored **on
your device** and are not uploaded to us. There is no account to create and no login. A small number
of optional or functional features can make network requests; each is described below.

## Who is responsible

ArenaScout is maintained by an individual developer (the "maintainer"). For any privacy question or
request, contact the maintainer through the
[ArenaScout status repository](https://github.com/TheUkiTendy/arenascout-status). A dedicated contact
address may be published here in future.

## What can leave your device — and why

- **Card detail lookups (on by default; you can turn this off).** ArenaScout ships with card data
  covering almost every card. For cards too new to be included, it can look them up online, sending
  only a **card identifier** to our card-data provider, [Scryfall](https://scryfall.com). No account,
  screen name, decks, match history, or other personal information is included. As with any internet
  request, the provider may receive your device's IP address. You can disable this in the app to keep
  ArenaScout fully offline.

- **Update and service notices.** The packaged app periodically retrieves a small, public file hosted
  on GitHub to check for available updates and important service notices. This request sends **no
  information about you, your account, or your matches**. As with any web request, it does reveal your
  device's IP address to the host (GitHub), whose own privacy practices govern that. The file is
  public and identical for every user.

- **Anonymous diagnostics (on by default; you can turn this off).** ArenaScout may send a small,
  anonymous diagnostic message containing only the application version and basic device information
  such as your operating system. **It carries no identifier** and cannot be used to single you out or
  recognise you across sessions — it simply helps us see which versions are in use and spot problems.
  You can switch it off in the app.

- **Optional usage statistics (off by default).** ArenaScout does not collect identifiable analytics
  unless you choose to turn them on. This feature is disabled by default and sends nothing extra
  unless you opt in. If you enable it, it additionally includes a random installation identifier (not
  linked to your name or identity) and a count of how many matches you have recorded — so we can tell
  how many people use ArenaScout over time. It never includes your Arena account, screen name, your
  opponents, your decklists, or any match details. You can opt out at any time, and you can request
  deletion of your installation identifier (see "Your rights and choices").

- **Feedback you choose to send.** If you use the in-app feedback feature, ArenaScout saves your
  report as a file **on your computer**. It contains the feedback you wrote, an optional name if you
  provide one, and a random installation identifier. **Nothing is sent anywhere automatically** —
  there is no in-app upload today; you decide whether and how to share the file with the maintainer. A
  private in-app submission option is planned, and this policy will be updated before any such feature
  is enabled.

## What we never collect

ArenaScout does not ask for or transmit your MTG: Arena login, password, or account details; your
real name; the contents of your matches, chats, or messages; or the identities of your opponents.
Opponent names are shown to you locally so you can review your own games — they are never uploaded to
us.

## Third parties

The features above involve a small number of third parties, each governed by its own policies:
[Scryfall](https://scryfall.com) (card-data lookups), [17Lands](https://www.17lands.com) (card-list
data bundled into the app; 17Lands does not receive anything from you), and
[GitHub](https://github.com) (host of the public update/status file). ArenaScout does not sell or rent
your personal information to anyone.

## Your rights and choices

Depending on where you live, you may have rights to access, correct, delete, or export your personal
information, to object to or restrict its processing, and to withdraw consent. Because ArenaScout
keeps your data on your own device, you are in direct control of most of it: you can view it in the
app and delete it by removing the app's local data. For anything we hold (for example, an installation
identifier from opt-in usage statistics), you can request deletion by **opening an issue** on the
[ArenaScout status repository](https://github.com/TheUkiTendy/arenascout-status) on GitHub (please
don't include sensitive personal details in a public issue — just reference your request, and we'll
follow up). You can also turn off online card lookups and anonymous diagnostics in the app, and opt-in
usage statistics are off unless you enable them.

## Data retention

**Important:** because ArenaScout is local-first, your match history, decks, and statistics live only
on your device. If you delete the app's data or uninstall ArenaScout, **all of that data is
permanently deleted and cannot be recovered** — there is no cloud backup. Consider exporting anything
you want to keep before uninstalling.

If you enable optional usage statistics, we intend to retain the associated records only as long as
needed to understand usage trends, and to purge identifiers from installations inactive for more than
12 months.

## Children

ArenaScout is not directed to children under 13 (or the minimum age required for consent in your
jurisdiction). It does not knowingly collect personal information from children.

## Regional notes

- **EU/EEA & UK (GDPR).** Where data is processed, our legal bases are: your *consent* for the
  optional (identified) usage statistics; and our *legitimate interests* (and providing the
  functionality you request) for the functional card-detail lookups, the update/safety check, and the
  anonymous diagnostics — which carry no identifier. You have the right to lodge a complaint with your
  local supervisory authority.
- **Canada (PIPEDA) & Quebec (Law 25).** Any non-essential collection (the optional usage statistics)
  is opt-in. We aim to collect the minimum necessary and to be clear about purposes.
- **California (CCPA/CPRA).** We do not sell or share your personal information, including for
  cross-context behavioural (targeted) advertising.

## Changes to this policy

We may update this policy as ArenaScout evolves. We aim to highlight material changes in the app.
