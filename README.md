# The Black Peach — Discord Application Privacy Archive

An **offline-ready static website shell** for the seven Discord apps associated with The Black Peach. The look is based on the dark peach/root imagery and the orange-black colour palette in your supplied branding screenshot. The portrait images come from your supplied `icons.zip`.

## Preview without publishing

Open `index.html` in Firefox/Chrome. All 7 tiles link to their own draft pages. No web server, scripts, fonts, analytics or paid services are needed.

## IMPORTANT: All seven policies are placeholders

**DO NOT use these draft pages as finished Privacy Policy URLs in the Discord Developer Portal.** Hooves of Thunder now documents the two permissions visible on its Discord authorisation screen and its login-only purpose, but its Worker/Cloudflare storage, retention and contact details still require confirmation. The other six applications still have outline placeholders. Once those reviews happen, the text in `/policies/*.html` can be replaced with accurate statements and dates. The home page's `00 policies published` statistic and the draft badges will need to be changed too.

## Application list (alphabetical)

1. Hooves of Thunder — Discord authentication for the horse racing website.
2. Icon — Trivia.
3. Kashima — UFC Betting.
4. Lady C — Chess.
5. Tomoka — Stardom Predictions.
6. Yagami — Various Games and Movie Queries.
7. Zombie Suzu — Testing (policy scope to be confirmed after code review).

## Publish on GitHub Pages, when ready

1. Create a **public repository** on GitHub (e.g. `discord-app-privacy`).
2. Upload **the contents of this folder** to the repository root (`index.html`, `assets/`, `policies/`, `.nojekyll`, `README.md`). Don't upload only the ZIP file.
3. In repository **Settings → Pages → Build and deployment**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
4. Your website will generally appear at `https://YOUR-USERNAME.github.io/discord-app-privacy/`. Each app's policy will live under `policies/{slug}.html`.
5. After the policies are **finalised**, link each correct policy URL in its matching Discord application settings.

Because the repository is public, all files uploaded to it (including the supplied icons) will be publicly visible. Check that you have the necessary rights to publish any photographs used as app icons.

## Website details

- The source design is pure HTML/CSS, no JavaScript or tracking.
- All links and assets are relative, so it also works offline and on project-style GitHub Pages URLs.
- The decorative hero artwork is a cropped, softened region of the screenshot you provided (without the Discord UI buttons).
- Pages currently contain `<meta name="robots" content="noindex, nofollow">` because they are drafts. That is optional to remove after final publication.
- Edit shared styling in `assets/style.css`; replace avatar images in `assets/icons/` as needed.

## Revision 2 — authentication details and hover stability

- Hooves of Thunder page now documents the two permissions shown by Discord: server member info (including nickname/avatar/roles) and basic username/avatar/banner profile access. It explains that the app is for login and server-role gating, not for chatting or reading messages. It **remains a draft** until Cloudflare/Worker session, retention and contact details are checked.
- Fixed the flicker that could appear at the lower edge of card artwork on pointer hover by eliminating `translateY` on the cards and `scale()` on the images. Those movements could make hover intermittently disengage near the card boundary and cause repaints at the image clipping edge. Cards now use a stationary border, background and shadow hover state.
- Added responsive styling to Hooves' permission summary; the other six policies are unchanged.
