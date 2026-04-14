# CLAUDE.md

This repository contains the privacy policy for the PocketOracle app, hosted via GitHub Pages at `https://corneloaie.github.io/pocketoracle-privacy/`.

## Source of Truth

The privacy policy must always reflect the actual data collection practices of the PocketOracle app. Before making any update to `index.html`, **read the main app repository** located at:

```
/Users/corneloaie/AndroidStudioProjects/PocketOracle
```

## What to Check in the Main Repo

When updating the privacy policy, inspect the following to ensure nothing is missing or outdated:

- **Analytics events** — `shared/src/commonMain/kotlin/com/corneloaie/pocketoracle/core/tracker/`
- **Third-party SDKs** — `shared/build.gradle.kts` and `androidApp/build.gradle.kts` (look for new dependencies)
- **Local storage keys** — `shared/src/commonMain/kotlin/com/corneloaie/pocketoracle/core/storage/`
- **Network/API calls** — any new Ktor or HTTP client usage
- **New features** — `shared/src/commonMain/kotlin/com/corneloaie/pocketoracle/` feature directories

## Update Checklist

When updating `index.html`:

1. Read the current `index.html` first
2. Check the main repo for any new SDKs, analytics events, or data flows
3. Update affected sections — do not rewrite sections that haven't changed
4. Update the "Last updated" date at the top
5. Commit with a clear message describing what changed and why
