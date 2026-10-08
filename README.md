# Yuki Ueno’s website

One-page academic website using the original [Minimal Light template](https://github.com/yaoyao-liu/minimal-light), as shown in its [demo](https://minimal-light-theme.yliu.me/).

The homepage layout, publication include, stylesheets, scripts, and favicons are copied unchanged from upstream revision `1ea07f39518ac44644406380c83da6f89037c4fc`. No custom layout or CSS overrides are loaded. The license is retained in `LICENSE-minimal-light`.

## Editing

- `_config.yml`: profile, links, and the template’s font/dark-mode settings
- `index.md`: About Me, Research Interests, News, and education within About Me
- `_includes/services.md`: service and teaching assistant experience
- `_data/publications.yml`: publications using the template’s original data format
- `images/` and `files/`: personal images and PDFs

Older page and collection sources remain in the repository but are excluded from the build. Former main navigation URLs redirect to the homepage. The one-page site omits the full research history, portfolio, blog, theses, and some older publications.

## Preview

```sh
bundle install
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

Open http://127.0.0.1:4000/. GitHub Pages builds the site using `_config.yml`.
