# Troubleshooting

## Menu bar icon is missing

- Run `swift run` from Terminal and check for errors
- Relaunch MacTools from the menu or quit and reopen

## Spotlight trigger fails

- Grant Accessibility permission to MacTools
- System Settings -> Privacy & Security -> Accessibility

## System Settings link not opening

- Pane IDs can change across macOS versions
- Update pane IDs in `Sources/MacTools/Resources/DefaultConfig.json`

## Icons disappeared in Finder

```bash
killall Finder
```
