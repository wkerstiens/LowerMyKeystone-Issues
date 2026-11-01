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

- Talk to Lindormi. A panel under her dialogue offers preset amounts, a custom amount and a cancel button.
- `/lowerkey <levels>` lowers your key by that many levels, for example `/lowerkey 3`.
- `/lowerkey stop` cancels a run in progress.
- `/lowerkey key <KEY|none>` binds a key to "Interact with Target" while a run waits for you.

Things worth knowing:

- Lindormi lowers one level per conversation. Between levels the addon shows a "Target Lindormi"
  button; left-click it, then right-click Lindormi (or press your interact key) to continue.
  Addons cannot open an NPC conversation themselves, so that step is yours.
- The run follows your real keystone level and stops at the target level or +2.
- The first run matches Lindormi's English option text. After that the option is remembered.

## Posting an issue

1. [Search the existing issues](../../issues) first; yours may already be there.
2. [Open a new issue](../../issues/new/choose) and pick *Bug report* or *Suggestion*.
3. Include, as far as you can:
   - what you expected and what happened instead
   - the addon version (the AddOns list on the character-select screen)
   - your keystone level before and after, and how many levels you asked for
   - what Lindormi's dialogue did after each level (goodbye page, closed, confirmation popup)
   - any Lua error text (an addon such as BugSack makes these easy to copy)
   - a screenshot, if it is a display problem
