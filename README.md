# The 80% Game

A mobile-friendly multiplayer number strategy game. Play alone against AI opponents or with friends and family.

## Deploy online (no laptop required)

1. Tap **[Deploy to Render](https://render.com/deploy?repo=https://github.com/fkieran-dev/The-80-percent-game)**.
2. Sign in to Render, connect GitHub if requested, and review the proposed web service.
3. Confirm it is set to the **Free** plan before approving.
4. Wait for Render to deploy. Open the `onrender.com` address shown on the service page.
5. Select **Play vs AI** or create a multiplayer room and share its code.

The `render.yaml` file configures the free Node.js service. No npm dependencies or API keys are required.

## Run locally

Requires Node.js 20 or later.

```bash
node 80-percent-game-render-one-file.js
```

Open http://localhost:3000 in your browser.

## Game options

- 2–10 participants, including AI-controlled opponents
- Solo play versus AI bots
- Private multiplayer rooms with secret submissions
- Survival and Tournament modes
- Automatic calculations, scoring, eliminations and progressive rules
- Mobile animations and reduced-motion support

## Limitations

This is a hobby prototype. Rooms and scores live in the server's memory, **not** in a database. A server restart or a free host spin-down can reset an active game. Render's free service may sleep when inactive, causing a delay on the first visit. Do not rely on this for permanent records.

The source is bundled in a single self-contained Node.js launcher. This simplifies uploading and deployment, but is less convenient to edit than the original multi-file project.
