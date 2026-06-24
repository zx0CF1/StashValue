# StashValue — GameHelper2 Plugin

**Pricing overlay plugin for Path of Exile 2.** Automatically evaluates and displays the market value of items inside your Stash and Inventory using real-time pricing data.

## What it does

- 💸 **Live Pricing**: Fetches background market prices using **poe2scout.com** or **poe.ninja**.
- 🎨 **Visual Overlay**: Draws clean pill-chip overlays directly on top of item slots.
- 📦 **Stash & Inventory pricing**: Separate configurable toggles to display prices on Stash slots, Inventory slots, or both.
- ⚙️ **Aesthetic Customization**: Easily configure font scale, color, display currency (Divine, Exalted, Chaos), and positional offsets.
- 🛡️ **Zero-Sync Lag**: Locates slots by walking the visible UI panel tree directly, ensuring pricing overlays update immediately without relying on slow or out-of-sync ServerData mappings.
- 🛠️ **Diagnostics**: Includes a debug diagnostic window and bounding box outlines to audit item entity addresses.

## Compatibility

| Attribute | Detail |
|---|---|
| **Game** | Path of Exile 2 (0.5.x+) |
| **GameHelper** | MordWraith Fork (.NET 10.0-windows) |
| **Tag** | `community`, `wip` |

## Install

1. Copy the `StashValue` plugin folder into your GameHelper `Plugins/` directory:
   ```
   <GameHelper>\
     Plugins\
       StashValue\
         StashValue.dll
   ```
2. Launch GameHelper.
3. Enable **StashValue** in the plugins list.

## Configuration & Saving

Open GameHelper → Plugins → StashValue:
- Settings are saved automatically to `config/settings.txt` inside the plugin directory whenever you adjust a toggle or slider in the UI.

## Credits & Upstream Attribution

This plugin was developed by **zx0CF1** through collaborative AI assistance (vibe-coding / prompt engineering) with acknowledgments to:
- **LootValue** (GameHelper2 upstream) for the overlay concept and visual reference.
- **RitualHelper** (originally by **caio** / *AutoRitualPricer*) for the mod parsing and price fetcher architecture.
