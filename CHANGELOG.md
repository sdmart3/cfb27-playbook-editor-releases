# Changelog

All notable changes to this project are documented here.
Versions follow [Semantic Versioning](https://semver.org/).

## [1.1.0] — 2026-09-26

### Added
- **Your own formation tabs.** Make as many as you like (Favorites, Red Zone, anything you name), and
  add, rename, reorder or delete them in step 4.
- **Custom sets at the top of the game's formations.** For example, a "Fav Split" as the first set in
  Shotgun, ahead of your usual order. A set from another formation keeps its own alignment, so an
  I-Form set in the Shotgun tab still lines up under centre.
- **Star adds to** in step 3 chooses where a starred play goes: one of your tabs, or a custom set at
  the top of any formation.
- **Import from a mod you built** (step 4). Moving from an older version, or lost your settings? Pick
  the "(playbook edits)" mod in your Mod Manager, keep the original mod under **Build on**, and your
  custom formations, custom sets and play order come back. Your current settings are kept aside.

### Changed
- Your play order is applied first and custom sets are added after it, so they stay at the top of
  their formation.
- Rebuilding from a playbook that already has custom sets replaces them rather than duplicating them.
- Existing Favorites carry over unchanged.

[1.1.0]: https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/tag/v1.1.0

## [1.0.3] — 2026-09-25

### Fixed
- **Choose the playbooks folder ran past the edge of the panel** in step 2. The buttons now size to
  fit and wrap on a narrow window.

[1.0.3]: https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/tag/v1.0.3

## [1.0.2] — 2026-09-25

### Fixed
- **No playbooks listed when the Documents folder has been moved** (for example to another drive).
  The app built the path to the saves folder by hand and never saw a moved Documents folder. It now
  asks Windows where Documents really is.

### Added
- **Choose the playbooks folder** button in step 2, for playbooks kept anywhere else. Pick the
  game's `saves` folder (or the "EA SPORTS College Football 27" folder above it) and the list
  switches straight away; the choice is remembered.
- Step 2 now says which folder the playbook list was read from, and what to do when it's empty.

[1.0.2]: https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/tag/v1.0.2

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
