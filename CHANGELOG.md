# Changelog

All notable changes to this project are documented here.
Versions follow [Semantic Versioning](https://semver.org/).

## [1.0.1] — 2026-09-25

### Fixed
- **"College Football 27 was not found" on EA app installs.** The EA app names the game's folder
  "EA SPORTS College Football 27" and the app only looked for "College Football 27". It now asks the
  Mod Manager's own settings where the game is first, then checks Steam's and the EA app's install
  records in Windows, and tries both folder names.
- **"Check again" could not find a fixed install without restarting the app.** A failed search was
  remembered for the whole session. It isn't any more.
- **A hand-edited config with single backslashes was silently ignored.** `C:\Program Files\...`
  typed straight into a config file now works.
- **The Mod Manager was reported as out of date whenever the game was not found.** Its cache can only
  be checked against the game, so until the game is found it now just says the Mod Manager was found.

### Added
- **Choose the game folder** button in step 1, shown when the game isn't found automatically. Pick
  the folder and the app saves it; no files to edit. Choosing the game folder with the Mod Manager
  button now says that's the game folder.

[1.0.1]: https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/tag/v1.0.1

## [1.0.0] — 2026-09-24

First public release. Every feature below has been run in the game.

### Added
- **Play order.** Put a custom playbook's formation sets, and the plays in each set, in the order
  you want on the play-call screen. One order serves all your custom playbooks.
- **Sort buttons.** A–Z for sets and plays; By type groups plays into runs, options, RPOs, play
  action, passes and trick plays by the game's own play types, with plays a mod adds in their own
  group.
- **Favorites formation.** Star plays from any formation; they appear in a new formation tab, each
  lining up and running as it does in its home set, motion included. Works with plays that a
  playbook mod adds.
- **Builds on your playbook mod.** Choose the mod that adds your sets or plays and the app builds a
  copy of it carrying your order and Favorites.
- **No setup.** Reads the game through the Mod Manager's cache and finds the install in Steam or the
  EA app. Self-contained: nothing to install.

[1.0.0]: https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/tag/v1.0.0
