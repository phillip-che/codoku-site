# codoku.app

Static site for [codoku.app](https://codoku.app), served by GitHub Pages.

- `/privacy` is generated from `docs/privacy.md` in the private `codoku` repository, which is the source of truth. Regenerate after a policy change:

```sh
npx --yes marked@latest --gfm -i docs/privacy.md -o body.html
```

then paste the output into `privacy/index.html` between `<main>` and `<footer>`, and update the date line in both places.

- `CNAME` binds the custom domain; DNS for `codoku.app` lives at the registrar.
