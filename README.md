# AI Connect: Research Meets Industry

Website for AI Connect 2026 (26–27 November 2026, Burg Frankenberg, Aachen).
Built with Jekyll and the Minima theme; the layout follows the
[EWRL18 site](https://euro-workshop-on-reinforcement-learning.github.io/ewrl18/).

## Editing content

| What | Where |
|------|-------|
| Dates, venue, application link, deadline, contact | `event:` block in `_config.yml` |
| Home page text | `index.md` |
| Program | `program.md` |
| Speakers | `_data/speakers.yml`, photos in `assets/images/speakers/` |
| Venue photo | `index.md` (Venue section), file in `assets/images/venue/`; CC BY 3.0, keep the credit |
| Organizers and their people | `_data/organizer_teams.yml` |
| Participating companies and their challenges | `_data/companies.yml`, logos in `assets/images/companies/` |
| Photos from past events | `_data/gallery.yml`, files in `assets/images/gallery/` |
| Hero and footer organizer and supporter logos | `_data/organizers.yml`, files in `assets/images/logos/` |
| Colours and layout | `assets/main.scss` |

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/ai-connect/>.

## Deploying

1. Push this repo to GitHub under the organization.
2. Settings → Pages → "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site appears at `https://<org>.github.io/ai-connect/`.

If the site gets a custom domain, or the repo is renamed to `<org>.github.io`,
set `baseurl: ""` in `_config.yml`.
