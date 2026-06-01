# Ironhold Arena

First playable browser prototype for a 2D isometric action RPG arena.

## Play

- Move: `WASD` or arrow keys
- Strike: `J` or left mouse
- Dash: `Space`
- Cleave: `Q` or `K`
- Restart after defeat: `R` or the restart button

## Cloudflare Deploy

This repo is set up for Cloudflare Workers.

```powershell
wrangler deploy
```

The deploy entry is `dist/worker.js`, configured in `wrangler.jsonc`.

## Notes

The prototype starts directly in the arena. Gameplay state is kept separate from the Phaser rendering path in the `src` files, while `dist/worker.js` is the deployable Worker bundle.
