# iTurnier

Organize football and other sports tournaments from your assistant using your existing iTurnier account.

## What you can do

- Read tournaments, teams, schedules, registration counts and preparation tasks.
- Preview schedules and edit them before the first match starts.
- Manage tasks, registration settings, sponsors and tournament or club pages.
- Prepare invitation mail; sending requires separate permission, a preview and your explicit confirmation.

You need an iTurnier **Pro** plan or access through a club with the **Verein** plan. Your role and plan apply to every
tool call. The assistant cannot change results or live scores. Stored player rosters, trainer and registration contacts,
invitation recipients and payment details are not returned by the connection. If you provide personal data in a
conversation and ask the assistant to enter it, that input can be sent to iTurnier.

## Connect your account

Install the plugin from your provider's directory when a listing is available, or import this package through a supported
custom-plugin flow. Connect the remote server at **https://iturnier.de/mcp**, sign in to your own iTurnier account and
review the permissions on the iTurnier consent page. Installation alone does not authorize access. Availability of custom
imports depends on your provider, plan and workspace.

For ChatGPT, you can also create a personal plugin under **Plugins → Add custom MCP server**, using the server address
above and OAuth. For Claude, use **Customize → Connectors → Add custom connector** if you only want the connection.
Start with read access and ask: “Show my iTurnier tournaments.”

### Install from the public repository in Claude Code

Run `/plugin install iturnier --marketplace timvallandi/iturnier-plugins` in Claude Code, then connect your iTurnier account
when prompted. The repository contains only the plugin's connection settings, instructions, documentation and logo.
For account-wide use on mobile, connect the remote server in your Claude account as described above. This repository
installation is separate from a public listing in the provider's directory.

Remote connections are account based; no local server, shell command or background process is installed by this plugin.
It bundles instructions and references and connects only to the public iTurnier MCP endpoint. It does not fetch your
conversation history, run local hooks or collect analytics. The iTurnier server returns tool results to your chosen AI
provider, whose own terms and privacy policy apply.

## Permissions and data handling

The available permissions are **Read**, **Organize** and **Send mail**. Mail permission is separate and disabled by default
on iTurnier's consent page. Revoke a connection at any time under **KI-Verbindungen** in iTurnier. Access tokens last one
hour; connections expire after at most 90 days and use rotating refresh tokens. iTurnier keeps connection metadata and
tool-call records without arguments or returned content for up to 90 days. The record identifies the tool, tournament,
result and duration. No recipient list, payment data or player roster is included in the plugin package.

- [Documentation and setup](https://hilfe.iturnier.de/verein-konto/ki-verbindungen)
- [Privacy Policy](https://iturnier.de/datenschutz)
- [Terms of service](https://iturnier.de/agbs)
- [Support](https://hilfe.iturnier.de/verein-konto/ki-verbindungen#hilfe-und-support) · [info@iturnier.de](mailto:info@iturnier.de)

## Deutsch

iTurnier hilft dir bei der Organisation von Fußball- und Sportturnieren. Verbinde dein eigenes Konto und entscheide,
ob der Assistent nur lesen, auch organisieren oder zusätzlich Einladungsmails versenden darf. Voraussetzung ist Pro oder
Zugang über einen Verein mit Tarif Verein. Tarif, Rolle und gewählte Rechte bleiben wirksam.

Zum Einstieg: „Zeige meine Turniere“ oder „Erstelle eine Spielplan-Vorschau, ohne sie zu speichern“. Ergebnisse und
Live-Spielstände sind geschützt. Gespeicherte Kader, Trainer- und Anmeldekontakte, Einladungsempfänger und Zahlungsdaten
werden nicht ausgegeben. Selbst eingegebene personenbezogene Daten können als gewünschte Änderung an iTurnier übertragen
werden. Den Zugang trennst du unter **KI-Verbindungen** jederzeit wieder.

Die Einrichtung für ChatGPT, Claude und Mobilgeräte ist in der verlinkten Anleitung beschrieben. Ein lokaler Import oder
eine bestandene Paketprüfung ist noch kein öffentlicher Verzeichniseintrag.

## License

This plugin package is distributed under the limited iTurnier plugin license in LICENSE. The hosted iTurnier service and
its application source are separate and are not included in this package.
