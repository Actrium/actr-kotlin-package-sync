# actr

Kotlin/Android package distribution repository for ACTR.

- Source of truth: [actr monorepo](https://github.com/Actrium/actr)
- Package sync repository: `Actrium/actr-kotlin-package-sync`
- Published Maven coordinate: `io.actrium:actr:<version>`

This repository owns the Kotlin package release workflows.
The release workflow clones `actr` at the requested source tag with `git clone --depth 1 --branch <tag>`, builds the Android artifacts from that temporary checkout, and publishes `io.actrium:actr:<version>` to GitHub Packages.

Do not copy the monorepo workspace into this repository, and do not develop product code here.
