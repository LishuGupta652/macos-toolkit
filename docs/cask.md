# Homebrew Cask

## 1) Host the ZIP

Upload the release ZIP somewhere stable (e.g., GitHub Releases):

```
MacTools-1.0.0.zip
```

## 2) Update the Cask Template

Edit:

```
Casks/mactools.rb
```

Update:

- `version`
- `sha256`
- `url`
- `homepage`

## 3) Install via Personal Tap

1. Create a repo named `homebrew-tap` (or similar)
2. Add your cask at:

```
Casks/mactools.rb
```

3. Install:

```bash
brew tap yourname/tap
brew install --cask mactools
```

## 4) Submit to Homebrew/homebrew-cask (Optional)

1. Fork `Homebrew/homebrew-cask`
2. Add `Casks/mactools.rb`
3. Open a PR
