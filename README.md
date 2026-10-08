# abhaysobhanan.github.io

Personal academic website of Abhay Sobhanan, built with Jekyll and served by GitHub Pages. There are no plugins beyond the ones GitHub Pages supports, so pushing to `master` is all it takes to publish.

## Updating the site

Almost everything you will want to change is a short entry in a YAML file in `_data/`. Copy an existing entry, edit it, commit.

| To change…                         | Edit                     |
|------------------------------------|--------------------------|
| Bio on the home page               | `_pages/about.md`        |
| News on the home page              | `_data/news.yml`         |
| Papers                             | `_data/publications.yml` |
| Research themes on the home page   | `_data/research.yml`     |
| Talks                              | `_data/talks.yml`        |
| Teaching                           | `_data/teaching.yml`     |
| Lab members                        | `_data/team.yml`         |
| Funded projects                    | `_data/grants.yml`       |
| CV page                            | `_data/cv.yml`           |
| Header links                       | `_data/navigation.yml`   |
| Name, email, address, profile links | `_config.yml`           |
| Colours, type, spacing             | `assets/css/site.css`    |

Each data file starts with a comment explaining its fields.

### Adding a paper

Add an entry at the top of the right group in `_data/publications.yml`:

```yaml
- id: my-new-paper            # used for links like /publications/#my-new-paper
  type: journal               # review | journal | conference
  title: "Title of the Paper"
  authors: "A. Sobhanan, C. Coauthor"
  venue: Transportation Science
  details: "60(1), 1–20"
  year: 2027
  topics: [learning]          # lists it under that theme on the home page
  links:
    doi: https://doi.org/...
    arxiv: https://arxiv.org/abs/...
    code: https://github.com/...
  abstract: >-
    Paste the abstract here, indented.
```

Your name (`me` in `_config.yml`) is set in bold automatically. Put † after a lab member's name to mark them.

### Moving a paper from "under review" to published

Change `type: review` to `type: journal`, then add `venue`, `details` and a `doi` link.

## Pages that are written as prose

`_pages/resources.md`, `_pages/prospective-students.md` and `_pages/beyond-research.md` are ordinary Markdown. Second-level headings (`## Heading`) hang in the left margin automatically.

`/beyond-research/` (the travel map, driven by `_data/travel.yml`) is live but not linked from the header; uncomment it in `_data/navigation.yml` to show it.

## Running locally (optional)

```sh
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Credits

Typeset in [Source Serif 4](https://github.com/adobe-fonts/source-serif) (SIL Open Font License), self-hosted from `assets/fonts/`. Originally forked from the academicpages template; the theme has since been replaced.
