# Nonlocality — DART REA dependency build

This repository holds a GitHub Actions workflow that downloads the **public** npm runtime dependencies for `rea-agents@6.4.0` on Linux x64 and packages them for an offline test environment.

No SNATCHER disc images, other game data, Ghidra distribution files, proprietary binaries, or research assets should be committed here.

The workflow runs on push to its workflow file or manually using **Actions → Build REA offline dependencies → Run workflow**. The generated build artifact is temporary and contains only npm-installed software.
