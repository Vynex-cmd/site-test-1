# site

Repo structure:

```
index.html
assets/
  images/
    pfp.png          ← your profile picture
    background.jpg   ← your custom background
  audio/
    background.mp3   ← your background music
```

## How to use

1. Drop your files into `assets/images/` and `assets/audio/` using the
   exact filenames shown above (`pfp.png`, `background.jpg`,
   `background.mp3`).
2. If a file is missing, that feature just falls back gracefully:
   - no `pfp.png` → shows your first initial instead
   - no `background.jpg` → default ambient gradient background
   - no `background.mp3` → volume control does nothing (no crash)
3. Different filename or extension? Update the matching path in the
   `CONFIG` object near the top of the `<script>` tag in `index.html`
   (e.g. `PFP_URL: "assets/images/pfp.png"`).

## Hosting on GitHub Pages

1. Push this folder's contents to a repo (root of the repo, or a
   `docs/` folder — your choice).
2. In the repo: **Settings → Pages → Source**, pick the branch/folder
   this lives in.
3. Your site will be live at `https://<username>.github.io/<repo>/`.

## Discord live status

Set `DISCORD_USER_ID` in `CONFIG` to your Discord user ID to show a
live status card (avatar, status dot, username, badges) powered by
the [Lanyard API](https://github.com/Phineas/lanyard). Your account
needs to have joined the Lanyard Discord server for this to work —
see the link above for the invite.
