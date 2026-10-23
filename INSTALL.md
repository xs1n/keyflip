# Installing KeyFlip

[Русский](INSTALL.ru.md) · [Back to overview](README.md)

Takes a couple of minutes. You need macOS 12 or later (Apple Silicon or Intel) with the Russian and English keyboard layouts enabled.

## 1. Download and drag to Applications

1. Download **KeyFlip.dmg** from the [latest release](https://github.com/xs1n/keyflip/releases/latest).
   If Chrome blocks the download, open Downloads (⌘⇧J) and click **Keep** — or download with Safari.
2. Open KeyFlip.dmg and drag **KeyFlip** onto the **Applications** folder.
3. Launch KeyFlip from Applications or with Spotlight (⌘ Space → “KeyFlip”).

## 2. Allow it to open (first launch only)

On first launch macOS shows this window (here in Russian — in English it reads *“KeyFlip” Not Opened*):

<p align="center"><img src="assets/macos-blocked-ru.png" width="320" alt="macOS window: KeyFlip Not Opened"></p>

That's expected: macOS shows it for any app without a paid Apple signature. KeyFlip is free and works offline — it doesn't send anything anywhere.

1. Click **Done**. ⚠️ Don't click *Move to Trash*.
2. Open **System Settings → Privacy & Security**.
3. Scroll down to the **Security** section. You'll see *“KeyFlip” was blocked to protect your Mac* — click **Open Anyway**.
4. Enter your Mac password, then click **Open Anyway** once more.

You won't see that window again.

> **No “Open Anyway” button?** It shows for about an hour after a launch attempt. Launch KeyFlip again, then go straight to Settings.
>
> Or run this in Terminal (it removes the “downloaded from the internet” mark from the app):
>
> ```
> xattr -dr com.apple.quarantine /Applications/KeyFlip.app
> open /Applications/KeyFlip.app
> ```

## 3. Allow keyboard access

KeyFlip has to see what you type — otherwise there's nothing to fix. On first launch it shows a window that walks you through it.

1. In the KeyFlip window, click the button that opens settings — **Privacy & Security → Accessibility** opens.
2. Switch on **KeyFlip**. If it isn't in the list, drag its icon from the KeyFlip window straight into the list (or click **+** and pick KeyFlip in Applications).
3. The KeyFlip window closes by itself and a keyboard icon ⌨️ appears in the menu bar. Done — start typing.

## 4. Make it yours (optional)

Click the ⌨️ icon in the menu bar → **Open KeyFlip…**, or just launch KeyFlip again:

- **General** — open at login, sound, which ⌥ Option key flips a word;
- **Dictionaries** — your own words (nicknames, brand names, slang) that KeyFlip leaves alone;
- **Exclusions** — apps where you don't want KeyFlip.

> The KeyFlip interface is in Russian.

## How to use it

- Just type: `ghbdtn` becomes «привет» after the space.
- **⌥ Option** (press and release) — flip the last word or the selected text to the other layout.
- **Double Shift** right after a fix — undo it.

## Updating

KeyFlip updates itself: once a day it checks for a new version and offers to install it — click **Установить** (Install), and it downloads the update, replaces itself and restarts. You can also check any time: menu bar icon → **Проверить обновления…** (Check for updates). Your dictionaries and settings stay.

By hand: download the new KeyFlip.dmg and drag KeyFlip to Applications, replacing the old one. After an update macOS may ask you to allow KeyFlip in Accessibility again: switch it off and on — and if that doesn't help, remove it with **−** and add it back with **+**.

## Uninstalling

1. ⌨️ menu bar icon → **Quit** (the last menu item).
2. Drag KeyFlip from Applications to the Trash.
3. Optionally, remove KeyFlip from **Privacy & Security → Accessibility** (the **−** button).

Something didn't work? [Open an issue](https://github.com/xs1n/keyflip/issues/new/choose) or write to [xsinus@gmail.com](mailto:xsinus@gmail.com).
