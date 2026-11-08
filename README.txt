Put workflows/flutter.yml into the root of the kgit-control repository (branch main),
replacing the old file. Commit it with the web editor on GitHub (do not build from the app first).

After that, every Flutter build in K-Git Studio uses this workflow. Future workflow fixes only need a new
file here and a higher "# kgit-workflow-version" number on line 2; no app release is needed.
An older file here is ignored by the app (version check), so a stale copy can no longer downgrade a build.
