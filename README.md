# Myya Design — GitHub Pages website

Static website ready to upload to GitHub. The **index.html** file must stay in the repository root.

## Publish
1. Create a new GitHub repository (for example `myyadesign`).
2. Upload **the contents of this folder**, not the ZIP file or a parent folder. Keep the `assets`, `css`, and `js` directories.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and click **Save**.
5. Your website will be at `https://YOUR-USERNAME.github.io/myyadesign/` (or `https://YOUR-USERNAME.github.io/` if the repository is named `YOUR-USERNAME.github.io`).

## Important: image files
The uploaded ZIP contained only a few image assets. Those present are now referenced locally from `assets/images/`. Other portfolio and animation images still use the original remote host. See `MISSING_IMAGES.txt` for the exact list. They can break if that host becomes unavailable. Download and upload copies **only if you have permission to use them**.

## Social sharing (OG image)
`assets/images/og.jpg` is included, but for reliable WhatsApp/Facebook sharing, change the `og:image` and `twitter:image` meta tags in `index.html` to the full HTTPS URL of your published GitHub Pages image. Example: `https://YOUR-USERNAME.github.io/myyadesign/assets/images/og.jpg`. Add an `og:url` meta tag with the full published site URL if needed. GitHub Pages cannot know your final URL before you choose a username/repository.

## Fonts
The original project referenced a local font file. This distribution uses a system fallback instead; if you have a webfont license, add your licensed font file separately and configure `@font-face`.

## Test locally
Run `python3 -m http.server 8000` in the project directory, then visit `http://localhost:8000/`.

No build tool, Node.js, or GitHub Actions are required.
