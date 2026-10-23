# Fun SMP Manager

**Developer:** Prakash  
**Copyright:** © 2022–2026, Developer Prakash

## Project status
This repository currently contains an **early plugin foundation**, not the complete promised server system.

Implemented in this starter:
- Paper plugin bootstrap
- `/funsmp status`
- permission-guarded `/funsmp reload`
- basic config/resources
- GitHub Actions build workflow

Not yet implemented: production anti-cheat and staff routing, Telegram bot commands/notifications, 40 playable worlds, full minigame/match systems, economy, claims, persistent identity/authentication, subscription billing/refunds, kits, shop, auction house, seasons, events, End War, and complete GUIs.

The included flight toggle signal is advisory-only and is **not a cheat determination**. The plugin does not automatically ban players. Do not use this starter as a production security or moderation system.

## Build
Requirements: Java 21 and Gradle 8.12.

```bash
gradle --no-daemon clean build
```

Output:
`build/libs/FunSMPManager-0.1.0.jar`

## GitHub Actions
Copy the `build.yml` from the companion **FunSMPManager-GitHub-Build-Files.zip** into:

`.github/workflows/build.yml`

Commit and push the repository. Open **Actions**, select **Build Fun SMP Manager**, then download the `FunSMPManager-JAR` artifact from a successful run.

## Install for testing
1. Use a disposable Paper test server compatible with the configured Paper API.
2. Copy the JAR into `plugins/`.
3. Start the server and inspect console output.
4. Never grant `funsmp.developer` to regular players.

## Commands
- `/funsmp status` — `funsmp.use`
- `/funsmp reload` — `funsmp.developer`

## Important
This is a starter project and has not been built or tested against a live Paper server in this response. Review and test before use.
