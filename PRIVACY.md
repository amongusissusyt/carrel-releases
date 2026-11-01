# Privacy

Carrel is a personal project made by one person. This page says plainly what it stores and what leaves your Mac. If anything here is wrong, that is a bug: please report it.

## What stays on your Mac

Everything you create lives in one folder, `~/Library/Application Support/Carrel/`:

- your spaces and open tabs, bookmarks, history, download list, habits, wins, deadlines, plan, events, clips and settings;
- the private urge journal (each note scrambled with a secret that your Mac's Keychain keeps for Carrel);
- a daily backup of the data file (last seven days), a log file, and any export you make.

Carrel has **no analytics, no tracking and no account**. It does not send what you browse, your notes or your habits anywhere. (An account system exists in the code but is switched off.)

## What Carrel connects to by itself

| What | Where | What is sent |
|---|---|---|
| Looking for a new version | `github.com` (the public `carrel-releases` repository), at start and every six hours | An ordinary web request. GitHub sees your IP address and that it was Carrel. Nothing about you or your data. You can switch this off in Settings → Updates. |
| "Update list" for the adult-site filter, only when you press it | `raw.githubusercontent.com` | An ordinary web request. |
| Family DNS (on by default) | Cloudflare's family DNS (`family.cloudflare-dns.com`) | The names of the sites you visit are looked up there, as they would be with any DNS service. Cloudflare's privacy policy applies. Turn it off in Settings → Protection if you prefer your own DNS. |
| Calendar links you add | The address you gave | An ordinary request for that calendar file. |

Websites you visit see you as any browser would be seen. Carrel does not hide your IP address and is not a privacy browser.

## The Keychain box

macOS may ask whether Carrel can use "Carrel Safe Storage" in your keychain. **That box belongs to macOS. Carrel never receives your Mac password**, and no one else does either: you type it into macOS, which uses it to unlock your Keychain for that one request. Carrel only gets back its own random secret, which it uses to scramble your private notes and any AI key you add, so other programs on your Mac cannot read them. Nothing about this leaves your Mac. If you choose Deny, Carrel cannot scramble or read those items and may behave oddly until you allow it.

## AI features (optional, only with your own key)

Carrel has no AI of its own. If you add a key from Anthropic, Google (Gemini) or OpenAI (or a compatible service), then **when you use an AI feature** Carrel sends this to the company you chose:

- the Assistant: your question, and, if you choose, the text of the page you are on, a screenshot of it, pictures you attach, and clips and open-page text for "My sources";
- syllabus reading: the text you import;
- plan estimates: your deadline titles and kinds;
- focus sessions: the words of your "if I feel the urge to…" line, to work out which sites it is about;
- reviewing a blocked site: the text of that page.

That company's own terms and privacy policy then apply, and you pay what it charges. Without a key none of this is sent. Keys are stored encrypted with the macOS Keychain and are never shown to web pages.

## Problem reports and diagnostics

"Report a problem" and "Copy diagnostics" (Settings → Help and feedback) put a text on your clipboard. It has versions, switch states, counts and the recent log, with web addresses, e-mail addresses, keys and your home folder name removed. **It never lists the sites you visited, your space names, notes or habits.** Nothing is sent automatically: you decide whether to paste it into a report.

## Exports and backups

An export is a plain file of your data (spaces, habits, deadlines, plan, notes and preferences). It never contains keys, your passcodes or protection settings. Daily backups are full copies of the data file, so they do hold encrypted key blobs and the passcode checks; they stay in the folder above. Keep exports somewhere you trust: they are readable by anyone who has the file.

## Removing everything

Quit Carrel, delete the folder above, and delete the app. To also remove the key it stores in the Keychain, open Keychain Access and delete "Carrel Safe Storage".

## What the protection features are, and aren't

The adult-content filter, focus sessions and passcode are speed bumps you set up for yourself. They are not a security product and can be got around by anyone with enough control of the Mac. See the README for the honest list of limits.
