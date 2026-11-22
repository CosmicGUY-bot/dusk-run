# Dusk Run 🏎️

A tiny retro racing game that runs in your browser. One HTML file, no dependencies, no build step.

**Vibe coded with [Claude](https://claude.ai):** I described the game in one sentence, and Claude wrote the code.

## Play

Open `index.html` in any modern browser. That's it.

## Controls

| Action | Keyboard | Touch |
|--------|----------|-------|
| Steer  | ← → or A D | ◀ ▶ buttons |
| Brake  | ↓ or S | ■ button |

Gas is automatic.

## How it works

- You start with 45 seconds. Each lap adds 20 seconds.
- Hitting a car or driving off the road slows you down.
- Your best distance is saved in your browser.
- The road is drawn with a classic pseudo-3D technique: the track is a list of segments, each projected onto a `<canvas>`.

## Tweak it

All settings are at the top of `index.html`:

- `MAX` is the top speed.
- `time=45` in `reset()` is the starting time.
- The `[enter, hold, leave, curve]` list defines the track bends.
- The `28` in `reset()` sets how many cars are on the road.

## Host it for free

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Branch**, choose `main` and `/ (root)`, then save.
4. Your game will be live at `https://<your-username>.github.io/<repo-name>/`.

## License

MIT, see [LICENSE](LICENSE).
