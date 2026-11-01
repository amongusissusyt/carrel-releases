# Carrel

**A browser for students who want to stop procrastinating and break the habits that pull them off task.**

Carrel is an early test version, made by one person (Ansh Sarawagi) for macOS. It is free. If you are reading this because you were asked to try it: thank you, and please tell me what breaks or confuses you.

## What it does

- **Focus sessions.** Press ⇧⌘F, write the one thing you are doing, and only the sites you allowed will open. Anything else makes you wait, so a passing urge has time to pass.
- **Blocks adult sites and distractions, and is slow to switch off.** The adult-content filter is always on. Turning off the blocking of adult-heavy platforms (Reddit, X, Discord…) takes 24 hours.
- **"Take a moment" for urges.** A slow-breathing pause, a private note, and an optional 30-minute lockdown of your distraction sites (social media, streaming, games).
- **A private journal behind its own passcode** for urges and what set them off. It stays on your Mac, scrambled so other programs cannot read it.
- **Habits and daily wins.** A month grid you can drag across, streaks, and one physical, one mental and one academic win a day.
- **Deadlines and a calendar you can edit.** Add things by typing "Maths tomorrow 4pm for 2h", drag them around, mark times that repeat every day.
- **A normal browser underneath:** tabs grouped into spaces, find, zoom, bookmarks, history, downloads.
- **Optional AI assistant**, only if you add your own key (Anthropic, Google Gemini and OpenAI-style services work). Nothing else needs AI.

## Download

**[Download the latest version](https://github.com/amongusissusyt/carrel-releases/releases/latest)**, then open the file for your Mac:

- **`arm64`** if your Mac has an Apple chip (M1, M2, M3, M4…).
- **`x64`** if it has an Intel chip. (Apple menu → About This Mac shows which.)

Open the `.dmg`, drag **Carrel** onto **Applications**.

### The first time you open it

Carrel is not signed with a paid Apple certificate, so macOS stops it once. This is normal for a small project, and you only do it once:

1. Open Carrel from Applications. macOS says it can't be opened. Click **Done**.
2. Open **System Settings → Privacy & Security** and scroll to the bottom.
3. Next to "Carrel was blocked", click **Open Anyway** and enter your Mac password.

(If you prefer Terminal: `xattr -dr com.apple.quarantine /Applications/Carrel.app`, then open it normally.)

After that, Carrel looks for new versions itself. When one is ready, click **Update available** and then **Install and restart**.

### If macOS asks about your Keychain

You may see a box saying **"Carrel wants to use your confidential information stored in 'Carrel Safe Storage' in your keychain."**

- **That box is made by macOS, not by Carrel.** Carrel never sees your Mac password. You type it into macOS's own box, and macOS does not pass it on.
- Carrel keeps one random secret in your Keychain, and uses it only to scramble your private notes (and any AI key you add) so other programs on your Mac cannot read them.
- Nothing is sent anywhere. There is no server and no account.
- Click **Always Allow**. You may be asked again after an update, because updates are not signed with a paid Apple certificate, so macOS treats each one as a new app.
- If you clicked **Deny**, quit Carrel, open it again and click **Allow**. Carrel may behave oddly until you do.
- To remove the secret later: open Keychain Access and delete "Carrel Safe Storage".

## Please read

- **It is a speed bump you set up for yourself, not a wall.** Someone who owns the Mac can get around it. There are two separate locks: a *privacy passcode* that keeps other people out of your private journal, and an optional *accountability code* that is most useful when a friend or parent types it in for you so you do not know it. Turning protection off always takes a 24-hour wait, and needs that code too if one is set.
- **It only runs on a Mac for now.** There is no iPhone, iPad, Android or Windows version yet. For your phone, use Screen Time → Content & Privacy → Web Content → Limit Adult Websites, with a Screen Time passcode someone else holds.
- **It is an early test.** Things will break. Your data is backed up daily on your Mac, and you can export it from Settings.
- **It is not medical advice.** If an urge feels out of your control, talking to a professional helps and is common.
- **Privacy:** no accounts, no tracking, nothing about what you browse leaves your Mac. The full list of what it connects to is in [PRIVACY.md](PRIVACY.md).

## Tell me what happened

In Carrel: **Settings → Help and feedback → Report a problem**. It copies a short report (versions and counts, never your sites or notes) and opens a page here where you can paste it and say what happened. Or [open an issue](https://github.com/amongusissusyt/carrel-releases/issues/new) directly.

Useful things to say: what you were doing, what you expected, which Mac and macOS version you have, and whether something confused you even if it worked.
