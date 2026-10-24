# Digitalinvitee – Cinematic 3D Wedding Invitation

## Run
ES modules need a web server (double-clicking index.html will not work):
```
cd digitalinvitee
python3 -m http.server 8000     # then open http://localhost:8000
```
Or deploy the folder to Netlify / Vercel / GitHub Pages / any host. Only Google Fonts needs internet (fallback fonts are used offline).

## Customize
- **Names, date, venue, events, story, WhatsApp number, maps link:** `js/config.js` (edit only this file).
  WhatsApp format: country code + number, no `+` (e.g. `919876543210`).
- **Intro video:** replace `assets/video/intro.mp4` (portrait 1080x1920 recommended; the supplied clip is trimmed to its first 2 seconds and its own audio removed) and `assets/images/poster.jpg` (fallback frame).
- **Background:** `assets/images/backdrop.jpg` (portrait) and `backdrop-wide.jpg` (landscape screens) – your rose frame.
- **Couple image:** `assets/images/couple.webp` (transparent cut-out) glides down as you scroll.
- **Gallery:** the six `gallery-*.jpg` are placeholder crops of your backdrop. Put your photos in `assets/images/` and list the names in `config.js`.
- **Music:** `assets/audio/music.mp3` (Ishq Sufiyana) starts the moment 'Tap to Open Invitation' is tapped (fade-in); the ♪ button mutes/unmutes. Replace the file to change the song.
- **RSVP:** sends a pre-filled WhatsApp message; the second button stores replies only in that guest's browser (no backend).

## Notes
Reduced-motion users and low-end phones get fewer particles, no 3D reveal, and lower pixel ratio.
