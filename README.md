# Forged Pet Happiness

A lightweight Forged WoW addon that improves Hunter pet status tracking through a clean, compact interface.

## Features

- Happiness bar based on in-game `1-3` pet happiness states
  - Green = Happy
  - Yellow = Content
  - Red = Unhappy
  - Gray = No pet / unknown
- Pet XP bar (`current/max`), including max-level display
- Pet info line: level + family (+ custom name when set)
- Loyalty text line
- Training points display (`TP:` label in white, value colorized)
  - Red = negative
  - White = 0
  - Green = positive
- Pet diet icon with tooltip
- Help icon with command tooltip
- Draggable frame
- Lock/unlock support
- Show/hide support
- Position persistence per character

## Installation

1. Close WoW.
2. Copy the addon folder to:
   - `World of Warcraft/Interface/AddOns/Forged_PetHappiness`
3. Ensure these files are inside that folder:
  - `Forged_PetHappiness_Utils.lua`
  - `Forged_PetHappiness_Diet.lua`
   - `Forged_PetHappiness.toc`
   - `Forged_PetHappiness.lua`
4. Start WoW and enable **Forged Pet Happiness** in AddOns at character select.

## Usage

The frame updates automatically based on pet/game events.

Slash commands:

- `/fph lock` — lock frame position
- `/fph unlock` — unlock and allow dragging
- `/fph reset` — reset frame position to default
- `/fph hide` — hide frame
- `/fph show` — show frame (re-centers to default)

## Vanilla/Forged Limitations

Some values depend on what Forged/Vanilla API returns at runtime.
When data is unavailable, the addon falls back to safe placeholders such as `Unknown` or `N/A`.

## Version

`0.1.0`
