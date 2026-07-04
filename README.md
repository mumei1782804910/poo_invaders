# 💩 Poo Invaders

A mobile-friendly arcade shooter in the spirit of Space Invaders. Help **Edmund** — a boy
with black hair and a trusty gun — blast waves of cute poo before they reach him. Get hit
and he loses a heart; run out of hearts and the poo explodes all over him!

Everything (graphics, chiptune music, sound effects) is generated in code, so the whole
game is a single `index.html` file with **zero dependencies and zero assets**. Perfect for
static hosting.

## How to play

- **Mobile:** drag anywhere on the screen to move Edmund. He fires automatically.
- **Desktop:** arrow keys (or A/D) to move, Space/Enter to start or retry.
- Shoot poo: **+10 points**. Clear a wave: **+50 points** and a faster, bigger wave arrives.
- Edmund has **3 hearts**. Falling poo blobs, poo touching him, or poo reaching the ground
  all cost a heart.
- Tap the 🔊 button to mute/unmute the music and sound effects.
- Your best score is saved in the browser.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `poo-invaders`).
2. Push this folder to it:

   ```sh
   git init
   git add index.html README.md
   git commit -m "Poo Invaders"
   git branch -M main
   git remote add origin https://github.com/<your-username>/poo-invaders.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Source: Deploy from a branch**, pick `main` and `/ (root)`, save.
4. After a minute your game is live at `https://<your-username>.github.io/poo-invaders/`.
5. Open that URL on your phone. For the full-screen arcade feel, use your browser's
   **Add to Home Screen** option.

> Note: mobile browsers only allow audio after a user gesture, so the music starts on the
> first tap ("TAP TO START").
