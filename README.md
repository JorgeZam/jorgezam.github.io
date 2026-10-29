# jorgezam.github.io

Personal academic website of **Jorge E. Zambrano Ibujés**, Assistant Professor at Universidad Diego Portales.

Live site: https://jorgezam.github.io

## Content

| Folder | What it holds |
|---|---|
| `_pages/` | Home (`about.md`), CV (`cv.md`) and the section index pages |
| `_publications/` | One file per publication (`category`: `manuscripts` or `conferences`; `selected: true` shows it on the home page) |
| `_teaching/` | One file per course (`category`: `instructor` or `assistant`) |
| `_advising/` | Theses supervised (`category`: `advisor` or `co_advisor`) |
| `_committees/` | Thesis committees (`category`: `member` or `external`) |
| `files/` | BibTeX files linked from the publications |
| `_config.yml` | Site settings, profile and social links |
| `_data/navigation.yml` | Top menu |

Changes pushed to `master` are published automatically by GitHub Pages.

## Running locally

With [Docker](https://www.docker.com/) installed, run this in the repository and open `localhost:4000`:

```bash
docker compose up
```

## Credits

Built with [Academic Pages](https://github.com/academicpages/academicpages.github.io), a fork of the [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/) Jekyll theme (MIT License, see `LICENSE`).
