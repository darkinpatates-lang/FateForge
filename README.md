# FateForge

FateForge is an infinite procedural character generator and lightweight battle sandbox. Characters are built from independent fate wheels, stored locally in the browser, compared in Vault, and simulated in Arena.

## V1.3.3.1 — Core Release

This is the clean FateForge core release. Experimental visual-generation integrations, temporary test backends, CORS proxies and AppDeploy files are intentionally excluded.

## Core Systems

### Forge

- Category-based fate wheel
- Race → Sub-Race dependency
- Primary and Secondary Ability
- Power Level, Potential, IQ, Personality, Weapon, Defense, Weakness, Status, Fate, Luck and Age
- Gender and Height wheels
- Six RPG stats: STR, DEX, VIT, INT, WIS and LUK
- Randomize and Full Character Generate
- Wheel Locks
- Sticky mobile category selector
- Specific Weapon Weakness target wheel

### Vault

- Character slots
- Rename, delete and activate characters
- Gender-aware random names
- Rarity and Absurdity Score
- RPG star ratings
- Character Card export
- Character comparison

### Arena

Arena is a narrative 1v1 combat sandbox. It considers RPG stats, Power Level, IQ, Potential, Luck, abilities, weapons, weapon traits, defense, weaknesses and specific-weapon weakness targets.

Weapons can provide traits such as ranged, blade, heavy, holy, exotic, critical chance, armor piercing, control, defense breaking and damage modifiers.

## Visual Generation

Visual generation is **not part of this core package yet**. It will be designed and added separately after the core release is restored and verified. No provider key, test-site dependency or temporary backend is included in this version.

The future visual system will keep all secret credentials outside the public GitHub Pages frontend.

## Localization

The application supports Turkish and English UI modes. GitHub-facing documentation is written in English.

## Local Data

Character data and settings are stored in browser `localStorage`. Important keys include:

- `wof_slots` — characters and active slot
- `wof_locks` — wheel lock state
- `wof_lang` — selected language
- `wof_theme` — selected theme

Clearing site storage can remove locally saved characters.

## PWA / GitHub Pages

The clean GitHub Pages package contains exactly five files:

- `index.html`
- `manifest.json`
- `service-worker.js`
- `icon.svg`
- `README.md`

The application uses relative paths so it can be hosted from the repository root.

## License

This project is an experimental/community-style project. Add an explicit open-source license if you decide to publish the code under one.
