# Publish the Washington geology website

The complete static website is in `docs/index.html`. Images, styles, and JavaScript are embedded; no dependency installation or build command is needed. The original downloadable `washington-geology.html` remains available at the repository root.

## Cloudflare Pages

1. In Cloudflare, open **Workers & Pages** and create a **Pages** project connected to GitHub.
2. Select `sphud/test` and use `main` as the production branch.
3. Choose an available project name; Cloudflare provides `PROJECT-NAME.pages.dev` for free.
4. Use **None** for the framework preset, leave the build command blank, and set the build output directory to `docs`. Keep the root directory at the repository root.
5. Save and deploy. Open the deployment URL and verify the map, a discovery card, and the passport.

Future commits to `main` automatically redeploy the connected Pages project. No custom domain is required.

## GitHub Pages alternative

1. Open repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/docs`, then save.
4. Wait for the Pages deployment to finish and open `https://sphud.github.io/test/`.

GitHub Pages is free for this public repository. Its default address is determined by the account and repository names. A separately registered custom domain is optional and normally costs money.
