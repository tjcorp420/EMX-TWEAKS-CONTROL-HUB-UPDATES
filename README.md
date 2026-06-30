# EMX Tweaks Control Hub Updates

This repo is the safe update source for the public EMX Tweaks Control Hub build.

The app checks `latest.json`, compares `version` to its current app version, shows the changelog, and opens the download/release link when the user clicks Download. It does not silently download or execute updates.

## Publish Flow

1. Build the public app with `npm run dist:emx`.
2. Upload the portable EXE to a GitHub Release.
3. Update `latest.json` with the new version, changelog, and release/download URL.
4. Commit and push this repo.
5. In the app's Advanced settings, set Update Manifest URL to the raw GitHub URL for `latest.json`.

Example raw URL:

```text
https://raw.githubusercontent.com/tjcorp420/EMX-TWEAKS-CONTROL-HUB-UPDATES/main/latest.json
```

Release page:

```text
https://github.com/tjcorp420/EMX-TWEAKS-CONTROL-HUB-UPDATES/releases/latest
```
