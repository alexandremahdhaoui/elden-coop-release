# Addendum to the Apache License 2.0

Copyright 2026 Alexandre Mahdhaoui.

This addendum sets the scope of the Apache License 2.0 in the file `LICENSE`. This addendum controls when the two texts disagree on what the license covers. The same scope applies to source code and to built binaries.

## The license covers the original work of this project

The Apache License 2.0 covers the work that the authors of Elden Coop wrote and that has no tie to Elden Ring. That work includes:

1. The launcher, its installer logic and its updater.
2. The method that loads a DLL into a process.
3. The generic hook, detour and pattern scanning code.
4. The session protocol between players, its message format and its checks.
5. The diagnostics, the report zip and the test harness.
6. The architecture, patterns and methods of this project.

## The license excludes everything tied to Elden Ring and FromSoftware

The license grants no right to Game Material. The owners of Game Material keep all their rights. Game Material means:

1. Elden Ring and its files, code, data, art, text, audio and save format.
2. The names and trademarks of Elden Ring, FromSoftware and their publishers.
3. Facts taken from the game. These facts include addresses, offsets, byte patterns, structure layouts, function signatures, event flag ids and text ids.
4. Source code that exists only to read, call, patch or describe those facts. The files `buildprofile.rs`, `rva.rs`, `version.rs`, `eventflag.rs`, `saveslots.rs`, `titlemenu.rs` and `gamesession.rs` in `eldenring-lib`, and the file `testdata/peeks.json` in `elden-coop-harness`, are examples.

## Third party work keeps its own license

The license never replaces the license of a third party. Any code or fact that comes from another project stays under the terms of that project. This rule covers `fromsoftware-rs`, `ERNativeUI` and every Rust crate this project uses.

## This project has no tie to FromSoftware

FromSoftware and its publishers did not make, approve or support Elden Coop. A player needs a legal copy of Elden Ring to use Elden Coop.
