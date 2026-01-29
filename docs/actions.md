# Actions

Each menu item uses a `type` and optional fields.

| Type | Required fields | Description |
| --- | --- | --- |
| `openSettings` | `paneID` | Open a System Settings pane |
| `openApp` | `path` | Open an app bundle path |
| `openURL` | `url` | Open a URL in the default browser |
| `shell` | `command` | Run a command (optional `arguments`) |
| `appleScript` | `script` | Run AppleScript via `osascript` |
| `clipboardCopy` | `text` | Copy text to clipboard |
| `clipboardClear` | - | Clear clipboard |
| `reloadConfig` | - | Reload config.json |
| `openConfig` | - | Open config.json in the default editor |
| `revealConfig` | - | Reveal config.json in Finder |
| `relaunch` | - | Relaunch MacTools |
| `quit` | - | Quit MacTools |
| `separator` | - | Insert a menu separator |

## Examples

### Open System Settings

```json
{ "type": "openSettings", "title": "Wi-Fi Settings...", "paneID": "com.apple.preference.network" }
```

### Run a Command

```json
{ "type": "shell", "title": "Restart Finder", "command": "/usr/bin/killall", "arguments": ["Finder"] }
```

### Run AppleScript

```json
{ "type": "appleScript", "title": "Trigger Spotlight", "script": "tell application \"System Events\" to keystroke space using command down" }
```

### Clipboard Shortcuts

```json
{ "type": "clipboardCopy", "title": "Copy Email", "text": "you@example.com" }
```
