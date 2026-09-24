# Saviru — web build

Play it: **https://dwimalatissa.github.io/saviru-web/**

A third-person open-world game set in Sri Lanka, about carrying light back
across an island the dark has taken.

The lamps went out. That is the whole inciting event, and it is deliberately
undramatic — nobody was cursed and nothing was punished. What comes in where the
light was is the **Andura**, from *අඳුර*, the everyday Sinhala word for darkness.
Somebody has to walk the country relighting the wayside shelters, and Saviru is
the one who can.

*Saviru* (සවිරු) is Sinhala for rays of light — the rays, not the sun. He is not
the source of what he carries; he is what a source gives off, and light that
travels far enough runs out. The rod works the same way, and that is where the
difficulty comes from.

## Playing it

Desktop and a keyboard, for now. Mouse-look needs pointer lock, and there are no
touch controls yet, so a phone will load it and then give you nothing to press.

| | |
|---|---|
| Move | `W` `A` `S` `D` |
| Look | mouse |
| Sprint | `Shift` |
| Jump | `Space` |
| Dodge | `Ctrl` |
| Attack | left mouse (light), right mouse (heavy) |
| Cast | `Q` |
| Change spell | `E` |
| Light a lamp | `F` |
| Become light, and fly | `R` |

Light is one meter and it pays for everything — the spells, and every second
spent flying. It refills at a lit lamp, in water, and in sunlight. Dark gathers
on you away from light, and past a threshold it starts doing real damage and
grounds you.

The columns standing over the horizon are lamps: violet where one has gone out,
gold where one is burning. They are the only thing in the game that tells you
where to go, and they fade as you approach.

This is a slice rather than a finished game. There is no story yet beyond the
lamps, and no ending.

## Ground rules

The game is set in a real place, and the source repository carries a document of
hard limits that overrides everything else in it: no Buddha image in any form,
no combat at any place of worship, and no real deity or named folk demon as an
antagonist. The Andura is formless and is nobody's demon. The *thovil* tradition
and its drummers are on the player's side, because turning a living healing rite
into monsters to be killed would get it exactly backwards.

## About this repository

This repo holds **only the exported browser build**. It is written by CI from a
separate private repository — no game source lives here, and nothing here is
edited by hand. The playable files sit on the `gh-pages` branch, which GitHub
Pages serves; that branch is force-pushed on every publish, so it never keeps
more than the current build.

Runs entirely in the browser, no install and no server. Needs WebGL 2, which
means a reasonably current desktop browser. The build is about 45MB, so the
first load is not instant.

The version in the bottom corner of the screen is the commit it was built from.
