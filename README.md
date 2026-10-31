# Shruti Pandey: personal site

A small Jekyll site for GitHub Pages. Pages: Home, Experience, Education, Awards, Projects.

## Run locally

One-time setup (macOS):

```
brew install rbenv ruby-build
echo 'eval "$(rbenv init - zsh)"' >> ~/.zshrc   # then restart the terminal
rbenv install 3.3.0
```

In the repo folder (`.ruby-version` picks 3.3.0 automatically):

```
ruby -v            # should print 3.3.0
bundle install     # first time only
bundle exec jekyll serve
```

Open http://127.0.0.1:4000/. The server doesn't auto-refresh on edits. Stop it with Ctrl+C and run it again, or add `--livereload`.

If a config change doesn't show up, run `bundle exec jekyll clean` first.

## Where to edit

| What | File |
| --- | --- |
| Name, email, LinkedIn and resume links | `_config.yml` |
| Home page intro and highlights | `index.md` |
| Jobs and internships | `_data/experience.yml` |
| Education | `_data/education.yml` |
| Awards | `_data/awards.yml` |
| Projects | `_data/projects.yml` |
| Header links | `_includes/header.html` |
| Colors and fonts (light/dark) | `assets/css/style.css` |

Each entry in a `_data` file is a `- title: ...` block. Copy an existing one to add more.

## Notes

- Every link opens in a new tab. A script at the bottom of `_layouts/default.html` sets this.
- The resume link must be shared as "anyone with the link can view", or visitors will see a sign-in page.
- Deploy: push to `main`. In the GitHub repo settings, set Pages to deploy from the `main` branch root.
