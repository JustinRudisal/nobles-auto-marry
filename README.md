# Nobles Auto Marry - Continued (1.1 Fix)

A fix and continuation of [Nobles Auto Marry](https://steamcommunity.com/sharedfiles/filedetails/?id=3606305941) by Fart Shartley, updated to work with Europa Universalis V patch 1.1.x.

## What it does

Automatically pairs unmarried nobles (and optionally other estate types) for marriage each month, keeping your court populated without manual effort. Configure eligibility, population limits, and notification settings through an in-game configuration panel.

## Changes from the original mod

- Updated `supported_game_version` from `1.0.*` to `1.1.*` — eliminates the launcher incompatibility warning
- Fixed AI auto-marry on_actions (`noble_auto_marry_for_ai_on_action`, `non_noble_auto_marry_for_ai_on_action`) that were defined but never connected to `monthly_country_pulse` — the AI auto-marry feature now actually fires
- Added missing `hint_noble_auto_marry` localization keys required by the situation system
- Fixed a missing closing quote typo in `noble_auto_marry.1.t` localization
- Fixed royal marriage reminders (event 57) ignoring the "hide notifications" setting; added a new independent `hide_royal_marriage_events` toggle so players can suppress royal reminders separately

## Features (inherited from original)

- Automatically marries unmarried nobles aged 18–25 each month
- Three eligibility modes: Unrestricted, Selective (few married relatives), Dynastic Preservation (dynasty-based filter)
- Optional marriages for Burghers, Clergy, Peasants, Dhimmi, Tribes, Cossacks estates
- Royal marriage reminder for crown estate characters eligible for royal marriage (independently toggleable)
- Population control: optionally kill surplus courtiers above a configurable limit
- AI auto-marry support (disabled by default)
- Full in-game configuration panel via the Situations screen
- Works on existing saves (situation activates within one month)
- Localization: English, French, Korean, Russian, Simplified Chinese, Turkish

## Compatibility

Requires EU5 patch **1.1.x**. Pure script mod — no base game file overwrites. Compatible with most other mods unless they also overwrite `monthly_country_pulse` in `on_action`.

## Credits

Original mod by **Fart Shartley** (Steam: [3606305941](https://steamcommunity.com/sharedfiles/filedetails/?id=3606305941)). This version fixes 1.1.x compatibility and known bugs.
