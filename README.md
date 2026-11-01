# LowerMyKeystone: issues and feedback

Public issue tracker for **LowerMyKeystone**, a World of Warcraft (Retail, Midnight) addon
that lowers your Mythic+ keystone by a chosen number of levels when you talk to Lindormi.

This repository holds no source code. It exists so bug reports and suggestions
have one place to live.

## Install

Get the addon from [CurseForge](https://www.curseforge.com/projects/1778257), or unzip it into
`World of Warcraft/_retail_/Interface/AddOns/` so the folder is `AddOns/LowerMyKeystone`.
Then reload the game.

## Using it

Screenshots are on the [CurseForge page](https://www.curseforge.com/projects/1778257).

- Talk to Lindormi. A panel under her dialogue offers preset amounts, a custom amount and a cancel button. The addon list button next to the minimap (or `/lowerkey show`) opens the same picker anywhere.
- `/lowerkey <levels>` lowers your key by that many levels, for example `/lowerkey 3`. `/lowerkey stop` cancels a run.
- `/lowerkey key <KEY|none>` makes one key target Lindormi and then open her dialogue while a run waits for you.
- `/lowerkey confirm`, `min`, `presets`, `resetpos` change the settings.
- `/lowerkey debug` prints the addon's state; `/lowerkey debug on` logs each step.

Things worth knowing:

- Lindormi lowers one level per conversation. Between levels the addon shows a "Target Lindormi"
  button (shift-drag to move it). Addons cannot open an NPC conversation themselves, so that step is yours.
- The run follows your real keystone level and stops at the target level or your minimum (+2 by default).
- The English option text is recognised automatically. On another language, open Lindormi's dialogue and
  run `/lowerkey learn`, then `/lowerkey learn <number>` for the option that lowers your key.

## Posting an issue

1. [Search the existing issues](../../issues) first; yours may already be there.
2. [Open a new issue](../../issues/new/choose) and pick *Bug report* or *Suggestion*.
3. Include, as far as you can:
   - what you expected and what happened instead
   - the addon version (the AddOns list on the character-select screen)
   - your keystone level before and after, and how many levels you asked for
   - what Lindormi's dialogue did after each level (goodbye page, closed, confirmation popup)
   - the output of `/lowerkey debug` (for a run that misbehaves, turn on `/lowerkey debug on` first)
   - any Lua error text (an addon such as BugSack makes these easy to copy)
   - a screenshot, if it is a display problem
