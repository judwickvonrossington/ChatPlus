# Chat+

Makes chatting in Ultimate Chicken Horse more fun, with three features:

1. **Emoji reactions** on any chat message
2. **Auto chat** (Hello, Goodbye, Well done, So close)
3. **Quick chat menu switcher** (treehouse, build mode, play mode, or automatic)

Every feature can be adjusted from the config menu (see *Settings* below).

---

## Feature 1: Reactions

Every chat message gets a small **+** button. Pick one of 10 faces and everyone who has Chat+ sees that face, followed by your name, next to the message.

The 10 faces: happy, laughing, surprised, sad, angry, heart eyes, thinking, cool, wink and blush.

- You get **one reaction per message**. Picking a new face replaces your old one.
- Reactions only show on messages that are still visible in chat.
- The **+** buttons appear when you open chat (you can change this to *always visible* in the settings).

### With a mouse
Open chat, click the **+** next to a message, then click a face.

### With a keyboard
1. Open chat. The newest message is highlighted (yellow **+**).
2. **Tab** moves the highlight down (newer messages), **Shift+Tab** moves it up (older messages).
3. Press **Space** (while the chat box is empty) to open the face picker.
4. In the picker, use **Tab** or the **arrow keys** to move, **Space** to send the reaction, **Backspace** to close the picker without sending.

If new messages arrive while you are highlighting one, the highlight stays on the message you picked.

---

## Feature 2: Auto chat

Chat+ can say things for you automatically. It uses the game's own quick chat lines, and it **never reacts to yourself**.

| When | You say |
|---|---|
| Someone joins the treehouse | "Hello!" (after 0.5 seconds) |
| You join someone else's lobby (not when you host) | "Hello!" (after 0.5 seconds) |
| Someone leaves the treehouse | "Goodbye" (after 0.5 seconds) |
| Someone finishes | "Well done!" |
| Someone dies on their last life | "So close!" |

Each one can be turned on or off separately. Auto chat works whether you are the host or a client, and it follows the game's own chat settings (if chat/emotes are turned off in the game, nothing is sent).

---

## Feature 3: Quick chat menu switcher

The game has three quick chat menus: **treehouse**, **build mode** and **play mode**. Their buttons overlap, which makes it easy to say "Goodbye" when you meant "Whoops...".

Pick which one you are on:

- **Automatic**: switches by itself (treehouse menu in the treehouse, build menu while placing pieces, play menu while running)
- **Treehouse**
- **BuildMode**
- **PlayMode**

---

## Settings

Open the config menu in game (F1 if you use BepInEx ConfigurationManager), or edit `BepInEx/config/com.chatplus.uch.cfg`.

**1. Auto Chat**
- Hello when someone joins treehouse
- Goodbye when someone leaves treehouse
- Well done when someone finishes
- So close when someone dies on last life

**2. Quick Chat**
- Quick chat menu: Automatic / Treehouse / BuildMode / PlayMode

**3. Misc**
- Plus buttons: WhenChatOpen / Always

---

## Good to know

- **Reactions need Chat+ on the host.** Reactions are shared through the host. Players who don't have the mod simply won't see them.
- **Auto chat and the quick chat menu only affect you.** They don't change anything for other players, and nobody needs the mod to see your auto chat messages.
- Chat+ doesn't change gameplay.

## Installation

Install with a mod manager (r2modman or Thunderstore Mod Manager). Or manually: install BepInEx 5, then put `ChatPlus.dll` in `BepInEx/plugins`.

## Troubleshooting

If something doesn't work, check `BepInEx/LogOutput.log` for lines starting with `Chat+`. Every hook the mod applies is logged there.

## Changelog

**1.1.2**
- Reactions with mouse and keyboard
- Auto chat, with a separate toggle for each message
- Quick chat menu switcher, including Automatic mode
