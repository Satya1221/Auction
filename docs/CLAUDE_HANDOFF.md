# Claude handoff — IPL Auction Android game

This repository is intended to hold the actual Android/Kotlin source for the IPL auction/cricket-management game. Claude should work from the checked-in source, not from a feature list alone.

## Before coding

1. Inspect the repository tree and confirm the Android project files are present (settings.gradle(.kts), root/app Gradle files, app/src/, manifest, Kotlin source, assets, and tests).
2. If only this handoff document or README is present, ask the owner to upload/push the project source first. Do not invent a replacement app.
3. Read the project README and inspect the actual implementation. Create a source-backed feature matrix: implemented, partial, missing, and needs device testing.
4. Start with a read-only audit; wait for approval before editing.
5. Preserve existing architecture and save compatibility. Never delete saves or make sweeping rewrites without explicit approval.
6. Make incremental changes, add tests for core auction/roster/match rules, and report exact build/test commands and their results. Do not claim Android device testing unless performed.

## Target game

An offline-first IPL franchise management game with player auction and bidding, roster and purse management, playing-XI selection, match simulation, tactical decisions, player development, academy/scouting, season fixtures/playoffs, stats, and durable multi-season saves.

Use a season-specific IPL ruleset; do not assume purse, squad cap, overseas limit, retention, or substitute rules are identical across seasons. Mark generated prospects as fictional and do not fabricate real-player statistics.

## Feature roadmap

The 70-feature roadmap is documented in docs/FEATURE_ROADMAP_70.md. It is a reconstructed design backlog, not proof that features are implemented. Validate every item against source code.

## Owner workflow (Android/Termux)

The owner may develop from a phone. Keep setup instructions practical for Termux/Debian, avoid unnecessarily heavy tooling, and explain missing SDK/build prerequisites. Do not assume Android Studio is installed.
