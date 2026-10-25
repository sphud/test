# Noah’s Projects

The static website is published from `docs`. No dependencies or build command are needed.

- `docs/index.html`: Noah’s Projects homepage.
- `docs/projects/washington-geology/index.html`: the complete interactive geology project, including the corrected painted PACIFIC OCEAN label and Social Studies report heading.
- `docs/assets/washington-map.png`: homepage preview artwork.
- `washington-geology.html`: a self-contained downloadable copy of the geology project.

## Cloudflare Pages deployment

Connect GitHub repository `sphud/test`, production branch `main`, framework preset **None**, blank build command, and build output directory `docs`. Leave the root directory at the repository root. Commits to `main` trigger the connected Pages deployment.

The homepage will be at `/`; the geology project will be at `/projects/washington-geology/`.

## Add more projects

1. Create a directory under `docs/projects/PROJECT-NAME/` containing an `index.html` and any local assets.
2. Add a project card to the project notebook section in `docs/index.html`, pointing to `projects/PROJECT-NAME/`.
3. Commit and push to `main`.

## Connect a custom domain

A custom domain must first be registered. In the Cloudflare Pages project, open **Custom domains**, choose **Set up a custom domain**, enter the registered hostname, and follow Cloudflare’s DNS instructions. Keep the DNS configuration for unrelated websites and services intact.

A custom domain does not guarantee access through a school’s filter. The school’s IT team may need to approve the site for classroom use.

## GitHub Pages alternative

In repository Settings → Pages, select **Deploy from a branch**, branch `main`, folder `/docs`. The default URL is `https://sphud.github.io/test/`. Relative project links and local assets work under that prefix.
