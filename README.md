# Carrel

**A browser for students who want to stop procrastinating and break the habits that pull them off task.**

Carrel is an early test version, made by one person (Ansh Sarawagi) for macOS. It is free. If you are reading this because you were asked to try it: thank you, and please tell me what breaks or confuses you.

## What it does

- **Focus sessions.** Press ⇧⌘F, write the one thing you are doing, and only the sites you allowed will open. Anything else makes you wait, so a passing urge has time to pass.
- **Blocks adult sites and distractions, and is slow to switch off.** The adult-content filter is always on. Turning off the blocking of adult-heavy platforms (Reddit, X, Discord…) takes 24 hours.
- **"Take a moment" for urges.** A slow-breathing pause, a private note, and an optional 30-minute lockdown of your distraction sites (social media, streaming, games).
- **A private, passcode-locked journal** for urges and what set them off, encrypted with your Mac's Keychain.
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

## Please read

- **It is a speed bump you set up for yourself, not a wall.** Someone who owns the Mac can get around it. It is most useful when a friend or parent types the passcode in for you so you do not know it.
- **It is an early test.** Things will break. Your data is backed up daily on your Mac, and you can export it from Settings.
- **It is not medical advice.** If an urge feels out of your control, talking to a professional helps and is common.
- **Privacy:** no accounts, no tracking, nothing about what you browse leaves your Mac. The full list of what it connects to is in [PRIVACY.md](PRIVACY.md).

## Tell me what happened

In Carrel: **Settings → Help and feedback → Report a problem**. It copies a short report (versions and counts, never your sites or notes) and opens a page here where you can paste it and say what happened. Or [open an issue](https://github.com/amongusissusyt/carrel-releases/issues/new) directly.

Useful things to say: what you were doing, what you expected, which Mac and macOS version you have, and whether something confused you even if it worked.
