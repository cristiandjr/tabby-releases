<p align="center">
  <b>English</b> &nbsp;·&nbsp; <a href="README.es.md">Español</a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/logo-dark.png">
    <img src="docs/assets/logo-light.png" alt="Tabby" width="440">
  </picture>
</p>

<h3 align="center">Keyboard navigation for macOS Mission Control</h3>

<p align="center">
  <img alt="macOS 14+" src="https://img.shields.io/badge/macOS-14%2B-111111?logo=apple&logoColor=white">
  <img alt="Swift 6" src="https://img.shields.io/badge/Swift-6-F05138?logo=swift&logoColor=white">
  <img alt="Free" src="https://img.shields.io/badge/price-free-2EA44F">
  <img alt="Status: alpha" src="https://img.shields.io/badge/status-alpha-F59E0B">
</p>

<p align="center">
  <a href="../../releases/latest/download/Tabby.zip"><img alt="Download for macOS" src="https://img.shields.io/badge/macOS-Download%20Tabby-0A5CFF?style=for-the-badge&logo=apple&logoColor=white"></a>
  <br>
  <sub>No installer: download the zip, open Tabby.app, done. Universal (Apple Silicon + Intel) · macOS 14+ · <a href="../../releases">all releases</a></sub>
</p>

<!-- Demo video: drag the .mp4 into any GitHub issue or pull request comment, copy the URL GitHub generates and paste it here on its own line. GitHub renders it as a player. -->

---

> [!NOTE]
> Tabby is in alpha: it works every day on the author's Mac, but expect rough edges. Bug reports are very welcome.

## What is Tabby?

Mission Control shows all your open windows at a glance, but choosing one still means reaching for the mouse or the trackpad. **Tabby lets you do it with the keyboard**, the same way you use ⌘Tab.

<p align="center">
  <kbd>⌃</kbd> <kbd>↑</kbd> &nbsp;➜&nbsp; <kbd>Tab</kbd> <kbd>Tab</kbd> &nbsp;➜&nbsp; <kbd>Return ↩</kbd>
  <br>
  <sub><kbd>Tab</kbd> &nbsp;➜&nbsp; <kbd>⌘</kbd> <kbd>2</kbd> &nbsp;sends the selected window to Desktop 2</sub>
</p>

1. **Open Mission Control** the way you always do: keyboard shortcut, F3, trackpad gesture or hot corner.
2. **Press <kbd>Tab</kbd>** to move through your windows, most recent first. <kbd>⇧</kbd> <kbd>Tab</kbd> goes back.
3. **Press <kbd>Return ↩</kbd>**: Mission Control closes and that exact window comes to the front.
4. **Or press <kbd>⌘</kbd> + a number**: <kbd>⌘</kbd><kbd>1</kbd>…<kbd>⌘</kbd><kbd>9</kbd> sends the selected window to that desktop, creating it if it doesn't exist yet. Mission Control stays open, so you can keep sorting.

Tabby doesn't replace Mission Control: it works on top of the native one. Outside Mission Control, it also takes over <kbd>⌘</kbd><kbd>Tab</kbd> to show every window one by one, like Windows does, including minimized ones and windows on other desktops, with <kbd>⌘</kbd><kbd>Q</kbd> closing just the selected window. You can turn that part off in Settings.

## Features

| | |
|---|---|
| ⌨️ **Keyboard first** | Tab, ⇧Tab and Return inside Mission Control, most recent window first. |
| 🎯 **The exact window** | Focuses the window you picked, even when several windows belong to the same app. |
| ✨ **See where you are** | The selected window lifts slightly with a soft spring and settles back when you move on. |
| 🗂️ **Send it to a desktop** | <kbd>⌘</kbd><kbd>1</kbd>…<kbd>⌘</kbd><kbd>9</kbd> moves the selected window to that desktop, creating it if it doesn't exist yet. |
| 🪟 **⌘Tab, window by window** | Tabby's app switcher lists windows, not apps. Hold ⌘, press Tab, release to switch. <kbd>⌘</kbd><kbd>Q</kbd> closes just the selected window. Turn it off in Settings if you prefer the standard one. |
| ⚙️ **Your shortcuts** | Change every shortcut in Settings. |
| 🪄 **However you open it** | Shortcut, F3, trackpad gesture or hot corner: Tabby doesn't depend on any of them. |
| 🍎 **Native** | Swift, SwiftUI and AppKit. A tiny menu bar app that stays out of your way. |
| 🔒 **Private** | No analytics, no accounts. It only listens to the keyboard while Mission Control is open, and its only network request is the optional check for new versions. |
| 💸 **Free** | Free for everyone, personal and commercial use. No accounts, no subscriptions. |

## Roadmap

- [x] **Spike 0:** validate the macOS capabilities Tabby relies on
- [x] **Mission Control by keyboard:** Tab, ⇧Tab and Return, the lift effect, desktop switches, Settings and the welcome tour
- [x] **Move the selected window to another desktop** with ⌘1…⌘9
- [x] **⌘Tab, window by window**, with ⌘Q closing just the selected window (0.1.0-alpha.7)
- [x] **Move to Applications** from the welcome tour (0.1.0-alpha.6)
- [ ] **v0.1.0:** first stable release, after a round of real-world use
- [ ] Arrow-key navigation based on the thumbnails' positions
- [ ] Number shortcuts (1–9) and window search
- [ ] Window switcher extras: a configurable shortcut (⌥Tab), ⌘` for the windows of the same app

## Download

Tabby is a single download, with no installer. Use the **Download** button at the top, or:

1. Download [**Tabby.zip**](../../releases/latest/download/Tabby.zip) from the latest release and open it to unzip **Tabby.app**.
2. Drag **Tabby.app** to your **Applications** folder. It also runs from Downloads, but *Launch at Login* needs it in Applications.
3. Open **Tabby.app**.

### The first time macOS blocks it

Tabby is free and isn't notarized by Apple, which requires a paid developer account. So the first time you open it, macOS says that Apple could not verify that Tabby is free of malware, and offers to move it to the Trash. Tabby is safe and its code is open, so:

1. Click **Done**. Don't move it to the Trash.
2. Open **System Settings → Privacy & Security** and scroll down to **Security**. You'll see *"Tabby" was blocked to protect your Mac.*
3. Click **Open Anyway**.
4. macOS asks again: click **Open Anyway**.
5. Enter your password or use Touch ID. **On a Mac with Touch ID, rest your finger on the sensor even if you see no dialog:** the request can wait silently, especially with an external display. Otherwise check your other display.
6. **If Tabby's icon doesn't appear in the menu bar after a few seconds, quit the stuck copy and open Tabby again.** The copy you opened before approving stays frozen, and macOS keeps sending every new double-click to it. Open **Activity Monitor**, select **Tabby**, click **ⓧ** → **Force Quit**, and open Tabby again. Your approval is already saved, so this time it starts right away. (Terminal: `pkill -9 Tabby; open ~/Downloads/Tabby.app`.)

Tabby opens, its icon appears in the menu bar, and a short welcome tour guides you through the **Accessibility** permission and a first try. You only do this once, although a new version downloaded from the internet may ask again.

## Troubleshooting

**macOS says it couldn't verify Tabby.** That's expected: Tabby isn't notarized by Apple. Click **Done** and follow the steps above (Privacy & Security → Open Anyway).

**I clicked Open Anyway and nothing happens. Activity Monitor shows Tabby at 0 % CPU.** macOS is waiting for your approval and the request can be silent: on a Mac with Touch ID, rest your finger on the sensor; with an external display, look at the other screen. If it stays stuck, the copy you opened before approving is frozen: force quit Tabby in **Activity Monitor** and open it again; your approval is already saved. In Terminal: `pkill -9 Tabby; open ~/Downloads/Tabby.app`. If it still won't start, the Gatekeeper service itself got stuck: run `sudo killall syspolicyd` in Terminal, then open Tabby again.

**Double-clicking Tabby does nothing.** Same cause as above: a frozen copy is catching every click. Force quit it and open Tabby again.

**There's no Open Anyway button.** It's only there for about an hour after macOS blocks Tabby. Open Tabby again so macOS blocks it, then go back to Privacy & Security.

**Tabby is in the menu bar, but nothing happens in Mission Control.** Tabby needs the Accessibility permission. **Settings → General** shows whether it's granted; grant it in **System Settings → Privacy & Security → Accessibility**. If Tabby is listed there and still doesn't work (common after replacing the app), turn its switch off and on again. **Diagnostics…** in the menu shows exactly what Tabby sees.

**⌘Tab still shows the standard app switcher.** Check that **Settings → General → "⌘Tab shows windows, not apps"** is on, that Tabby is enabled, and that it has Accessibility (the switcher uses the same keyboard access as Mission Control). Inside Mission Control, ⌘Tab stays native on purpose. In password fields (Secure Input) macOS blocks every keyboard tool, Tabby included.

**The selected window doesn't lift, or ⌘Tab shows icons instead of thumbnails.** Both need the optional Screen Recording permission: **Settings → General → Allow Screen Recording**. Without it, Tabby works with a plain highlight and app icons.

**"Launch at login" is greyed out.** Tabby is running from Downloads or another folder. Use **Settings → General → Move to Applications**, or drag Tabby.app to Applications with the Finder and open it again.

**⌘1…⌘9 says the window is on all desktops.** That app is assigned to every desktop in macOS: right-click its Dock icon → **Options → Assign To → None**.

**I switched desktops inside Mission Control and the list looked wrong for a moment.** Tabby waits until macOS finishes the switch (about a second) before rebuilding the list; keys you press meanwhile are applied once it's ready. If it stays wrong, open an issue with the Diagnostics report.

**Tabby asked to be approved again after an update.** Every download goes through Gatekeeper once. Your permissions are kept, because every version is signed with the same certificate. On a Mac that never shows the approval prompt, you can skip Gatekeeper for the new copy before opening it: `find ~/Downloads/Tabby.app -print0 | xargs -0 xattr -d com.apple.quarantine`.

**You have several copies of Tabby.** Keep only the one in Applications and delete the rest, including the zip, so you always open the same one.

**How do I report a problem?** **Diagnostics…** in the menu → **Copy Report** → paste it in a [new issue](../../issues/new). The report has no window titles, keystrokes or personal data.

## Privacy

macOS requires Accessibility permission for apps that detect Mission Control, read window information and focus windows that belong to other apps. Tabby uses it for exactly that:

- It only listens to the keyboard while Mission Control is open, plus ⌘Tab (and the keys that follow it) while the window switcher is on.
- It never records or sends what you type.
- It has no analytics and no accounts. Its only network request is a check for new versions: when it starts and every 12 hours it reads the latest release from GitHub. Nothing about you is sent, and you can turn it off in Settings.
- **Screen Recording is optional** and only powers the lift effect. Tabby captures the windows of the current display while Mission Control is open, keeps the images in memory and drops them when it closes. Nothing is saved or sent. Without it, Tabby works the same with a plain highlight.
- **Diagnostics…** in the menu shows exactly which permissions Tabby has and what it detects, and its report has no personal data.

## Requirements

macOS 14 Sonoma or later · Apple Silicon or Intel

## Feedback

If something doesn't work, open **Diagnostics…** in the menu, click **Copy Report** and paste it in a [new issue](../../issues/new). The report has no window titles, keystrokes or personal data.

## Support Tabby

Tabby is free for everyone, made with ❤️ in Argentina 🇦🇷. If it saves you time every day, you can buy me a coffee: every contribution helps add features and keep Tabby up to date with each new macOS.

- **Mercado Pago** alias (Argentina): `cristiandjr.mp`
- **USDT** on the Tron (TRC20) network, from anywhere in the world: `TFUMsNxJGjum96MKHLfwabf8MTxpVuZLBx` — send only USDT on TRC20 to this address.
- Starring the repo ⭐ and sharing Tabby with a friend helps a lot too.

## License

Tabby is free to download and use, for personal and commercial purposes, under the [Tabby License](LICENSE). Tabby is proprietary software: its source code is not public, and the Tabby name, logo and icon belong to their author. Versions up to 0.1.0-alpha.4 were published under the MIT License, which keeps applying to those versions only.
