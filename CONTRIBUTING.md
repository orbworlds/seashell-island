# Contributing to Seashell Island

Thanks for wanting to help. Bug fixes, new things to do and ideas are all welcome as pull requests.
Merged changes go live on [Orb](https://orbworlds.com/orb/seashell-island?utm_source=github&utm_medium=readme&utm_campaign=seashell-island) within about 15 minutes.

Before you open one:

- **Try it.** `npm start` runs it locally with Orb's runtime. Open a second tab to check anything
  multiplayer, and have a look on a phone too (your browser's device mode is a good start).
- **Run the tests.** `npm install` once, then `npm test`. It loads the world in a headless browser and fails if anything throws. Every pull request runs it as well.
- **One file.** The game is `index.html`, and it should stay that way: no build step, no new dependencies. Libraries come from a CDN at a pinned version, like three.js.
- **Leave `window.orb` optional.** It only exists on Orb and in the kit, so write `orb?.store` and
  not `orb.store`, and the game still works when opened on its own.
- **Orb's files.** `orb-kit/`, `test/pw.mjs`, `test/smoke.mjs`, `package.json`, `docs/cover.webp`, `docs/screenshots/` and `.github/workflows/test.yml`
  are kept up to date by Orb's bot. If one needs changing, open an issue.

Not a coder? [Remix it on Orb](https://orbworlds.com/orb/seashell-island?remix&utm_source=github&utm_medium=readme&utm_campaign=seashell-island) and describe your idea instead. If it turns
out well, open an issue with the link.
