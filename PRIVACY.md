# Winland privacy

Winland has no accounts, no analytics and no tracking. It does not send anything to its developers.

## What stays on your PC

| Data | Where |
|---|---|
| Quick notes | `%APPDATA%\Winland\notes.json` |
| Settings | `%APPDATA%\Winland\settings.json` |
| Winland Pro license key (if you add one) | Inside `settings.json`. It's checked on your PC; Winland never sends it anywhere. |
| Anthropic API key (if you add one) | Inside `settings.json`, encrypted with Windows DPAPI so only your Windows account can read it |

Delete the `%APPDATA%\Winland` folder to remove all of it. In the Microsoft Store version (Winland for Windows), Windows keeps these files in the app's own folder and removes them when you uninstall it.

## What Winland reads

- **Now playing:** the song title, artist, album art and playback position that apps report to Windows' media controls. Winland only displays this; it does not store or send it anywhere.
- **Your Start menu app list:** to find AI apps you have installed. Nothing leaves your PC.
- **Touchpad finger positions (Winland Pro, only while trackpad gestures are on):** used on the spot to recognise the volume and brightness gestures. They are never stored or sent anywhere.
- **Key presses (Winland Pro, only while keyboard sounds are on):** Winland notices each key going down and up so it can play a click. It only checks whether it's an ordinary key, a wide key (Enter, Backspace, Shift…) or the space bar, then forgets it. What you type is never recorded, stored or sent anywhere.
- **Which window is in front:** only to check whether it's full-screen, so the island can hide.

## What leaves your PC

- **Buying Winland Pro in the Microsoft Store version:** the purchase is handled entirely by Microsoft under [Microsoft's privacy statement](https://privacy.microsoft.com/privacystatement). Winland only asks Windows whether Pro is owned; it never sees your payment details.
- **Built-in Claude chat:** only if you use it, your messages are sent to Anthropic's API using your own API key, under [Anthropic's privacy policy](https://www.anthropic.com/legal/privacy).
- **AI apps and websites** you open from the island are separate apps with their own privacy policies. Winland just opens them.

## Questions

Email winland.app@gmail.com, or open an issue at https://github.com/monmeeth-env/Winland-download/issues.
