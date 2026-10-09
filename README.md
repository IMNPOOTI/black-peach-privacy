# The Black Peach — Discord Application Privacy Archive

A static privacy-policy website for the seven Discord applications associated with **The Black Peach**.

## Privacy policies

Each application has its own privacy policy, prepared from the application's described functionality and, where applicable, its supplied source code and configuration. The pages explain the data used by each application and provide a contact for privacy and deletion requests.

| Application | Purpose | Policy |
| --- | --- | --- |
| Hooves of Thunder | Discord authentication for the horse racing website | [Privacy policy](policies/hooves-of-thunder.html) |
| Icon | Trivia | [Privacy policy](policies/icon.html) |
| Kashima | UFC betting with virtual currency | [Privacy policy](policies/kashima.html) |
| Lady C | Chess puzzles and ratings | [Privacy policy](policies/lady-c.html) |
| Tomoka | STARDOM wrestling predictions | [Privacy policy](policies/tomoka.html) |
| Yagami | Games and movie queries | [Privacy policy](policies/yagami.html) |
| Zombie Suzu | Restricted testing application | [Privacy policy](policies/zombie-suzu.html) |

**Privacy contact:** [blackpeach-privacy@proton.me](mailto:blackpeach-privacy@proton.me)

Policies should be updated whenever an application's features, data handling or retention practices change.

## Website

- Static HTML and CSS; no JavaScript, analytics, visitor accounts or third-party fonts.
- The design uses The Black Peach branding, supplied app icons, and a custom favicon.
- Responsive layout with stationary hover effects.
- Relative links allow the site to work locally and on GitHub Pages.
- Only the website's public assets and policies belong in this repository. **Do not upload bot source code containing credentials, tokens, config secrets or databases.**

To preview locally, open `index.html` in a web browser.

## Publish on GitHub Pages

1. Upload the contents of the website folder to the root of the public `black-peach-privacy` repository: `index.html`, `assets/`, `policies/`, and optionally `README.md` and `.nojekyll`.
2. In **Settings → Pages**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and **Save**.
3. The website address will be: **https://imnpooti.github.io/black-peach-privacy/** (once GitHub Pages finishes publishing).
4. Each Discord app's **Privacy Policy URL** should point directly to its corresponding page under `https://imnpooti.github.io/black-peach-privacy/policies/`.

When updating a privacy policy, replace only the relevant HTML file in the repository and commit the change. GitHub Pages will republish automatically.

### Note about this README

This `README.md` is shown on the **GitHub repository page**, below the file list. It is **not** the privacy website homepage: the website homepage is `index.html`.
