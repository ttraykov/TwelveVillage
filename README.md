# The Village — World of Twelve community concept

A responsive, static **DOFUS-inspired fan-forum prototype**, drawing on the server-by-server community idea of the former Imps Village and modern forum conventions. A separate portfolio project; not affiliated with Ankama or the original Imps Village.

## Preview locally

Open `index.html` in a browser. No installation or build step required. Fonts are loaded from Google Fonts when internet access is available; system fallbacks are provided.

## What's interactive

- Choose a server from the selector or quick chips. Global discussions are visible everywhere.
- Browse forum categories (General, Buy & Sell, Player Services, Guides, Recruitment, Safety, Updates).
- Search sample threads by title, description, author, or server.
- Sort by latest activity, replies or views, and open example discussion details.
- Bookmark discussions **for the current page session only**.
- Preview future login/registration, reply, new-thread, and promoted-listing flows.
- Use the responsive menu on smaller screens.

**Nothing is connected to a database.** All discussions, member names, view counts, listings, sponsor examples and other activity are fabricated for the prototype. The login and registration forms do not transmit or store credentials. Do not enter real passwords.

## Future build

Authenticated accounts and roles; real database-backed boards and threads; server profiles, moderation/reporting, attachments, user reputation, service verification, sponsored listings and payments (only where permitted by game and payment-provider rules), notifications, search, and administration.

## GitHub Pages

For tested setup commands using the intended `ttraykov/TwelveVillage` repository, see [DEPLOY-GITHUB.md](DEPLOY-GITHUB.md).

This static site is compatible with Pages project-site hosting. Create a new repository, add the contents of this folder at the root, and use **Settings → Pages → Deploy from a branch → main / (root)**. The `.nojekyll` file is included.

## References and attribution

Historical inspiration: Imps Village, which was an independent English-speaking DOFUS community forum (discussion references: https://www.reddit.com/r/Dofus/comments/1cbdxuo/). General modern forum patterns: https://docs.xenforo.com/manual/forums/nodes-forums. Server name references: official Ankama status page https://status.ankama.com/. This concept uses an original CSS/SVG visual identity. No official game art is included.

This project is an independent fan concept. **DOFUS and associated trademarks are owned by Ankama.** Do not imply official endorsement. Review Ankama's current community and marketplace policies before offering real goods or services.


## Video guides & PvP previews (v2)

The home screen contains a small video gallery and a **Videos & PvP** discussion board. Four fictional video-thread examples demonstrate PvP highlights, a Xelor class guide, dungeon tutorials, and team fights. All thumbnails are original CSS visuals; no actual footage is embedded or uploaded. Clicking a card opens a sample thread and a non-playing player placeholder.

**Future implementation:** authenticated creators should be able to attach videos to threads, add titles, descriptions, categories, server tags, timestamps and captions; receive replies and moderation reports; and share a playable stream. Consider using external video embedding (with embed privacy controls) or managed video storage/transcoding and moderation, rather than storing raw videos directly in the app database. Implement rate limits, file validation, copyright reporting, player consent, and storage quotas before enabling uploads.
