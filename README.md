# Personal Website

This repository preserves a legacy personal-website scaffold and the engineering notes around it. The executable source is based on JR Cologne's Gulp Starter Kit rather than a finished personal portfolio, so the repository is maintained as an implementation/reference archive instead of presenting the starter demo as a completed website.

## What is here

- `src/` — the starter example source, including raw HTML, Pug, Sass, JavaScript, and a sample image.
- `gulpfile.js` — the historical Gulp 4 build pipeline, organized into named build tasks.
- `bin/install.js` — the starter CLI installer, retained with safer process execution and documented responsibilities.
- `docs/PRODUCT_AND_ENGINEERING_CASE_STUDY.md` — repository-specific analysis of the scaffold, constraints, and product/engineering direction.
- `package.json` / `package-lock.json` — the legacy dependency set retained for reproducibility and security history.
- `LICENSE` — the upstream MIT license and attribution for the JR Cologne starter-kit code.

Generated output belongs in `dist/` and should be rebuilt from `src/` rather than committed as a second source of truth.

## Development

The package exposes the original Gulp workflow:

```bash
npm install
npm run build
npm start
```

This is a legacy toolchain. Dependency or runtime upgrades should be treated as a separate modernization task and validated against the Pug, CSS-preprocessor, Webpack/Babel, image, and BrowserSync steps together.

## Source conventions

The source tree intentionally contains only files that contribute to the example or explain how the starter works. Empty Sass/Pug placeholders and unrelated root-level compiled specimens have been removed.

Authored JavaScript and build functions carry short descriptions explaining their responsibility. Generated/minified output should be documented through its owning build task rather than edited by hand.

## Upstream attribution

The scaffold is derived from the JR Cologne Gulp Starter Kit / `@jr-cologne/create-gulp-starter-kit`, originally authored by JR Cologne and distributed under the MIT License. The upstream copyright and license text are preserved in `LICENSE`.

## Repository status

Treat this repository as a legacy scaffold plus case study, not as the canonical modern portfolio. Repository documentation should describe what actually exists here and should not be rewritten by automated README generators or machine-profile tooling.
