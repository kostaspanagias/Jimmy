# Zombie Apocalypse

A top-down pixel-art zombie shooter that runs in the browser. The whole game is in a single `index.html` file, with no build step or dependencies.

## Running

Open `index.html` in a browser. Some browsers restrict audio or storage on `file://` pages. If music or high scores don't work, serve the folder over HTTP instead:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Controls

| Action | Key |
| --- | --- |
| Move | W A S D |
| Aim / shoot | Mouse / left click (hold to fire) |
| Pause / resume | Space or Esc |

The game also pauses automatically when the window loses focus.

## Gameplay

- There are 3 levels with 100, 200 and 400 zombies. Later levels add fast runners and tanky brutes.
- Weapon pickups (machine gun, shotgun) last 60 seconds. Bandages and painkillers restore health.
- Your top 5 scores, language (English or Greek), volume, music track and character are saved in the browser's `localStorage`.

## Project layout

```
index.html        # game: markup, styles and all JavaScript
assets/audio/     # background music tracks (selectable in Settings)
```
