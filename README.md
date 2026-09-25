# Playbook Editor

A Windows app for **EA Sports College Football 27** custom playbooks. It puts your formation sets
and plays in the order you want on the play-call screen, and adds a **Favorites** formation that
holds the plays you call most, taken from any formation.

It reads your own files, on your own machine. Nothing is uploaded anywhere.

**[Download the latest release](https://github.com/sdmart3/cfb27-playbook-editor-releases/releases/latest)**

---

## Install

1. Download `PlaybookEditor-vX.Y.Z-win-x64.zip` from the releases page.
2. Unzip it anywhere: Desktop, Downloads, a USB stick. It does not install anything.
3. Run **`START Playbook Editor.bat`**.

Windows SmartScreen will warn you on first run, because the app is not code-signed.
*More info → Run anyway.*

### Requirements

- **Windows 10 or 11 (64-bit).** Everything else the app needs is inside the folder. The window uses
  the Microsoft Edge WebView2 runtime, which ships with Windows 10 and 11; if it is missing, the
  launcher opens the same tool in an Edge app window instead.
- **College Football 27**, found automatically in Steam or the EA app. If it isn't, click **Choose the
  game folder** in step 1 and pick the folder the game is installed in.
- **The Mod Manager, opened at least once since the last game update.** The app reads the game
  through the Mod Manager's own cache, so there is nothing else to set up.

---

## What it does

| | |
|---|---|
| **Play order** | Drag sets and plays into the order you want. One order serves all your custom playbooks. |
| **Sort buttons** | **A–Z** sorts sets or plays by name. **By type** groups a set's plays into runs, options, RPOs, play action, passes and trick plays, using the game's own play types. Plays added by a mod get a group of their own. Every play shows its type. |
| **Favorites** | Star any play and it goes into a new formation on the play-call screen. Each favourite keeps the formation it was designed for, so it lines up and runs exactly like the original, motion included. Plays from mods work too. |

### How to use it

1. Pick your custom playbook. They are read from the game's `saves` folder in your Documents; if
   yours are somewhere else, click **Choose the playbooks folder**.
2. Under **Build on**, choose the playbook mod you have enabled (one that adds sets or plays), or the
   game's own play sheet if you don't use one.
3. Order your sets and plays, and star your favourites.
4. **Build.** The mod lands in the `mods-to-import` folder beside the app. Import it in the Mod
   Manager. If you built on a mod, disable the original and enable the new copy: it carries
   everything the original does.

Build again whenever you change the order or your Favorites, after a game update, and after the
playbook mod you build on is updated.

### Is it safe?

- **Your playbook is never changed.** Favorites go into a **new** playbook written beside the one you
  picked, with a fresh gameplan and audibles. If that name already exists, the app asks first and
  backs up the old file.
- **Built mods go to `mods-to-import` only.** Never copy files into the Mod Manager's own Mods folder.

---

## Verifying your download

Each release includes a `.sha256` file. To check the zip you downloaded:

```powershell
Get-FileHash .\PlaybookEditor-v1.0.2-win-x64.zip -Algorithm SHA256
```

Compare the result with the published checksum.

---

## Reporting a problem

Open an [issue](https://github.com/sdmart3/cfb27-playbook-editor-releases/issues). Helpful to
include: the version, which step, what you expected, and what happened. If the app showed an error
message, paste it.

## About this repository

This repo holds **releases only**. The source is maintained privately.

## Use and redistribution

Free to download and use. This is not open-source software and no licence to redistribute or modify
it is granted. It includes third-party components under their own licences, and it reads game data
formats belonging to their respective owners. Not affiliated with or endorsed by EA.
