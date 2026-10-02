# Prosight Graph — releases

Built releases of Prosight Graph for macOS (arm64, x86_64): one archive with its own Python and the graph's program as
bytecode. DevDeck installs the latest one on a new Mac, and an installed graph updates itself from here once a day.

The source is private. A release is built here by `.github/workflows/release.yml` from a tag of the source repository
(`vX.Y.Z`): it reads the source through a read-only deploy key, builds on macOS runners and publishes the archive,
its `.sha256` and `release.json` (version, commit, API).
