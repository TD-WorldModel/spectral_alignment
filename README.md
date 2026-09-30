# World Modeling through Spectral Alignment

A standalone research blog based on the supplied SpectralAlignment.pdf and the abstract figure and all eight accompanying graphs. Authors and affiliations follow the supplied LaTeX source. Holger Molin and William Peng share an equal-contribution group; their order is randomized on each page load.

## Preview

Run `python3 -m http.server 4173 --bind 127.0.0.1 --directory dist` from this folder and open http://127.0.0.1:4173/.

## GitHub Pages

Repository: [TD-WorldModel/spectral_alignment](https://github.com/TD-WorldModel/spectral_alignment). `.github/`, `dist/`, and this README are at the repository root. The site is ready to deploy without a build step, package installation, or custom secrets.

To publish:

1. Push this folder's contents to the repository's `main` branch. If its publishing branch has another name, update `branches` in `.github/workflows/pages.yml` first.
2. In the repository, open **Settings → Pages → Build and deployment** and select **GitHub Actions** as the source.
3. Open **Actions → Deploy to GitHub Pages → Run workflow** for the first deployment. Later changes to `dist/` on `main` deploy automatically.

The workflow uploads only `dist/`.

All site assets use relative paths, so the same files work at `https://td-worldmodel.github.io/spectral_alignment/` or a root-level Pages site. There is no repository name or custom domain to fill into the website itself. The live URL appears in the completed deployment.

The workflow follows [GitHub's custom Pages workflow guide](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).

## Editing

The website is plain HTML, CSS, and JavaScript, without a build step. KaTeX and its fonts are bundled locally, so math rendering needs no external requests. Edit `dist/index.html`, `dist/styles.css`, and `dist/script.js`. Original PDFs and high-resolution rendered figures are in `dist/assets/`.

Features include responsive section navigation, a temporal-kernel explorer, borderless enlarged vector figures over a blurred background, dismissed by clicking or pressing Escape, expandable ablations, and print styling. The illustration shows the raw kernel before centering or tempering; it does not simulate training results.

All research claims and numbers are drawn from the supplied manuscript. The three reference websites informed the presentation style, not the scientific content. A compact theory section at the end gives the four main theorems and the appendix result on kernel dominance, with assumptions and a link to the paper for proofs. Publication status follows the supplied manuscript.
