# Fusebreak — playtest build

A top-down dig-and-blast stealth game. You are underground, everything around
you can be dug through or blown up, and the people looking for you hunt by noise
and by line of sight.

---

## Download

### ➡️ [Get the latest build](../../releases/latest)

Two downloads on the release page — pick yours. No installer for either: unzip
it anywhere and run it.

| | File | Run |
|---|---|---|
| **Windows** 10/11, 64-bit | `Fusebreak-<version>-win64.zip` | `Fusebreak.exe` |
| **Linux**, 64-bit | `Fusebreak-<version>-linux-x86_64.zip` | `Fusebreak.x86_64` |

There is no Mac build. Sorry.

### Windows will stop you the first time

You will get a blue box saying **"Windows protected your PC"**.

> Click **More info**, then **Run anyway**.

That happens because the file is not code-signed yet — signing certificates cost
money and this is a prototype going round a small test group. It is not a sign
that anything is wrong with the download. Your antivirus may grumble for
the same reason; if it quarantines the file, please tell me rather than fighting
it, because that is genuinely useful to know.

### On Linux

Double-click `Fusebreak.x86_64`, or run `./Fusebreak.x86_64` from a terminal in
its folder. If it will not start, some unzip tools drop the "executable"
permission — `chmod +x Fusebreak.x86_64` puts it back. It needs a desktop (X11
or Wayland) and a graphics driver that does OpenGL 3.3 — any card or integrated
chip from the last decade.

**The Linux build is new.** It passes its own automated tests on Linux, but
nobody has played it on a Linux desktop yet. If it does not start or looks
wrong, that is exactly what I need to hear — with your distro and graphics card.

---

## What I need from you

**20–40 minutes.** Start a **New Campaign** — it opens on a short cinematic
(hold **Esc** to skip it), then a training mission, then the first real level.
That opening stretch is the part I care about most.

After that, keep going if you want. There are forty levels and an endless mode
(Relentless) in there. The later levels have had far less play than the early
ones. Wander if you feel like it — just tell me which bit you mean.

Play it the way you would play something you had bought. **If you get stuck,
stay stuck for a while before giving up.** How you get unstuck is the single
thing I am most trying to learn.

### Then tell me

Not a checklist. Just play, then say whatever you remember.

1. **Talk me through anything you tried that nobody told you to try.**
   Especially if it worked. Especially if it did not.
2. Was there a moment where you thought *"oh, I could do X"*? What was X?
3. **Would you have played another level?** Honest answer. "No" is a genuinely
   useful result and will not hurt my feelings.
4. Anything you expected to be able to do and could not.
5. Anything that felt unfair, unclear, or like the game breaking.

What you *did* is more useful to me than what you thought of it. If you can
record yourself, or just scribble notes as you go, even better.

---

## Where to send it

**[Discord](https://discord.gg/JEpgakwmsQ)** — quickest, and you do not need a
GitHub account.

Once you are in, post in **#game-testing**. It is a forum channel, so please
**start your own thread** rather than adding to somebody else's — one thread per
person keeps each account of playing readable end to end, which is most of what
makes this useful.

A good thread is one post when you finish saying what you did, and separate ones
for anything that broke. Do not tidy it up; half-formed is fine.

Or open an [issue](../../issues) if you would rather.

### If something breaks

**Press F8** (or pause with **Esc** and choose **Save a Report**). The game
saves one zip with a screenshot, the build and your computer, where you were,
what you had been doing, your saves and the game's logs, and opens the folder
it is in. Attach the zip to your thread with a line about what happened.
Nothing is sent anywhere — the zip stays on your machine until you post it.

If the game ever closes by itself, the next time you start it the main menu
says **Fusebreak closed unexpectedly** and can open the log folder. Please
attach the newest log.

The game keeps a log of the levels you play (`playlog.jsonl`, beside your
saves) so a report can show what happened. It stays on your machine.

Saves, logs and reports live in:

```
Windows:  %APPDATA%\Godot\app_userdata\Fusebreak\
Linux:    ~/.local/share/godot/app_userdata/Fusebreak/
```

If the game ever loses your progress there will be a file in there ending
`.unreadable`. Please send me that one; it is the only record of what happened.

---

## Controls

On screen at the bottom left for the first minute, then they fade out of the
way. Press **H** to bring them back, or to dismiss them for good. **Every one
of them can be rebound** in Options → Controls — keyboard and controller
separately.

---

## Things I already know

Please do not spend your feedback on these:

- **All the art and audio is generated by code** rather than drawn or recorded,
  so it looks and sounds like exactly that. Do say if something is hard to
  **read**, though — that is a real problem, not a matter of taste.
- The later levels have had much less play than the first ones.
- It has hardly run on any machine except mine, and the Linux build not at all.

Everything else is fair game. Please be blunt — a polite playtest is a wasted
one.
