# Chord

A fast, keyboard-first desktop email client that runs on your computer. Every action has a shortcut, mail is stored locally so everything is instant, and there are no Chord servers between you and your mail. If you turn AI on, it tells you which conversations need you, drafts replies in your voice, and runs errands over email ("get me quotes for aluminium sheets from suppliers near me"). Nothing is sent until you press send. You can also leave AI off completely.

This repository holds Chord's installers and update files. Chord checks here for new versions and updates itself (from 0.2.1 on).

## Download

Get the newest version from **[Releases → Latest](https://github.com/HadiHassan22/chord-releases/releases/latest)**, then pick the file for your computer:

| | File |
|---|---|
| macOS (Apple Silicon: M1 and later) | `Chord_<version>_aarch64.dmg` |
| macOS (Intel) | `Chord_<version>_x64.dmg` |
| Windows | `Chord_<version>_x64-setup.exe` |
| Linux | `Chord_<version>_amd64.AppImage`, `Chord_<version>_amd64.deb` or `Chord-<version>-1.x86_64.rpm` |

## Install

Chord isn't signed with Apple or Microsoft certificates yet, so both ask once before the first launch.

- **macOS:** open the `.dmg` and drag Chord to Applications. Open it once. When macOS says it can't check the app, go to **System Settings → Privacy & Security** and click **Open Anyway**. Or run `xattr -dr com.apple.quarantine /Applications/Chord.app` in Terminal.
- **Windows:** run the installer. If SmartScreen appears, click **More info**, then **Run anyway**.
- **Linux:** `sudo apt install ./Chord_*.deb`, or `chmod +x Chord_*.AppImage` and run it.

### Updates

From version 0.2.1, Chord checks for new versions when it opens and every few hours. It downloads them in the background and asks before restarting. You can turn this off in **Settings → General → About**. If you have 0.2.0, install the latest version by hand once. Your mail and settings are kept.

## Signing in with Google

Gmail and Google Workspace accounts connect with **Continue with Google**. Google is still verifying Chord, so during sign-in you'll see **"Google hasn't verified this app"**. This is expected. Click **Advanced**, then **Go to Chord**, and approve access. Keep the Gmail box ticked, because Chord needs it to read and send your mail. Your sign-in stays in your computer's keychain.

## Privacy

Chord has no servers. Your mail, settings and sign-ins stay on your computer, and AI requests go straight from your computer to the provider you choose. Read the full [privacy policy](https://chord.example/privacy). <!-- TODO: replace chord.example with Chord's real domain once there is one. -->
