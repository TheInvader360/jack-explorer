### Features

- [x] walk around map (tile based)
- [x] move between linked map rooms (i.e. cross screen boundary)
- [ ] text panel (e.g. action descriptions, debug output, etc)
- [ ] teleport between locations (i.e. enter/exit dungeon)
- [ ] info panel (e.g. arrows, gold, keys, health, bestiary, etc)
- [ ] item pickup (e.g. arrows, gold, key, health, macguffin, etc)
- [ ] player attack (i.e. shoot arrow in faced direction)
- [ ] simple enemies (random movement, shoot on line of sight, random loot, etc)
- [ ] player health and gameover/restart
- [ ] locked doors (unlocking consumes a key)
- [ ] boss fight (high health, bullet hell, etc)

### Intro

* Our land is dying.
* Only the power of the Uniforce can restore it.
* It is hidden in the old abandoned mine...
* Protected by a powerful dragon!
* You, our saviour, must venture into the mine...
* Defeat the dragon...
* Retrieve the Uniforce...
* Activate the Monolith...
* And save our land!
* (press the space key to start)

### Rooms

1. (link 2)
* player can move around
* player can complete game by interacting with monolith if macguffin held

2. (link 1&3)
* player can loot magic box to replenish arrows (limited arrows in quiver, unlimited arrows in magic box)

3. (link 2&4)
* player has a single enemy to contend with (kill or avoid)

4. (teleport 5)
* player has multiple enemies to contend with (one is blocking path and must be defeated to continue)

5. (teleport 4&6)
* player has multiple enemies to contend with

6. (teleport 5)
* player has boss to contend with (blocking path and must be defeated to continue)
* player can loot chest to get macguffin

### Notes

if player loses all health, gameover - replace player sprite with grave spite, display message in text panel:

```
You were defeated! Press the space key to start again...
```

if player defeats dragon, display message in text panel:

```
You defeated the dragon! Now find the Uniforce...
```

if player gets macguffin, display message in text panel:

```
You found the Uniforce! Now take it to the Monolith...
```

if player interacts with monolith, display message in text panel:

```
The Uniforce activated the Monolith and our land was saved! (if has macguffin)
The Uniforce can activate this Monolith to save our land! (else)
```

on completion, display a success slide in game window, display message in text panel:

```
A WINNER IS YOU! Press the space key to exit...
```
