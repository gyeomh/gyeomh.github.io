# gyeomh.github.io

Personal website of Gyeom Hwangbo — https://gyeomh.github.io

Built with [Jekyll](https://jekyllrb.com/), using the template by
[Martin Saveski](https://github.com/msaveski/www_personal).

## Updating the content

Everything you normally need to change lives in `_data`:

| File                       | What it holds                                            |
| -------------------------- | -------------------------------------------------------- |
| `_data/main_info.yaml`     | Name, title, email, profile photo, social links, CV path |
| `_data/publications.yaml`  | Publication list (`selected: y` shows it in the Selected tab) |
| `_data/experience.yaml`    | Vitæ timeline entries                                    |

The bio text is in `index.html`. Layout and styling live in `_layouts/`,
`_includes/`, and `libs/custom/my_css.css`.

The standalone LEGO-Eval project page is served from `LEGO-Eval/`
(https://gyeomh.github.io/LEGO-Eval/) and is copied to the built site as-is.

## Running locally

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the
site and publishes `_site` to the `gh-pages` branch that GitHub Pages serves.

## External libraries

- CSS: [Skeleton](http://getskeleton.com), [Skeleton Tabs](https://github.com/nathancahill/skeleton-tabs),
  [Timeline](https://codepen.io/NilsWe/pen/FemfK), [Font Awesome](https://fontawesome.com/),
  [Academicons](https://jpswalsh.github.io/academicons/)
- JS: [jQuery 3.1.1](https://jquery.com/)
