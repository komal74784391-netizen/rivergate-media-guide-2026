# Rivergate Media Guide 2026

Static site for the Rivergate Roller Derby League's 2026 season media guide.
The site is built from Markdown files under `clubs/`, one page per club.

## Repository layout

- `clubs/<club-slug>.md` — one media-guide entry per club
- `_data/navigation.yml` — order of the club pages in the site menu
- `assets/` — shared site artwork (league crest)
- `index.md` — landing page

## Club entry front matter

Every club page starts with YAML front matter:

```yaml
layout: club
club: "Club Name"
city: "City"
founded: 2011
home_venue: "Home Venue"
primary_color: "#112233"
summary: "One-paragraph blurb"
kit_repo: "club-kit-repository"
back_to_back:
  HA: 0
  AH: 0
  HH: 0
  AA: 0
  total: 0
```

`kit_url` is optional and only belongs on the page when the club's published
design package is available to link. `back_to_back` holds the club's season
consecutive-day game-pair counts (see the season stats brief for the key
definitions).

## Local preview

```bash
bundle exec jekyll serve
```
