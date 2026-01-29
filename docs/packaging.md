# Packaging & Release

## Build

```bash
./scripts/build.sh
```

## Package the .app

```bash
./scripts/package_app.sh 1.0.0
```

Optional:

```bash
BUNDLE_ID=com.yourname.mactools ./scripts/package_app.sh 1.0.0
```

## Create Release ZIP + SHA

```bash
./scripts/release.sh 1.0.0
```

Output:

```
dist/MacTools-1.0.0.zip
```

## Signing & Notarization (Recommended)

```bash
./scripts/sign_notarize.sh dist/MacTools.app "Developer ID Application: Your Name" you@example.com TEAMID APP_SPECIFIC_PASSWORD
```

Notes:

- Use a Developer ID Application certificate
- Gatekeeper will warn on unsigned apps
