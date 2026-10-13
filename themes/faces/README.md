# FACES theme

A small custom Hugo theme for emilyburchfield.org (direction B: warm and landscape-led).
No external theme or JavaScript; one stylesheet (`static/css/faces.css`) and plain templates.

## Where things live (site folder)
| What | Where |
|---|---|
| Home page text (hero line, section intros) | `content/_index.md` |
| Research steps (the four home-page rows and their pages) | `content/research/<step>/index.md` + `featured.jpg`; order by `weight`; step 2 uses `panel: "timeline"` instead of a photo |
| Full publication list | `content/publication/_index.md` (one `## YYYY` per year, newest first). The home page shows its first four entries |
| Highlighted papers | `content/publication/YYYY_XX/` (`index.md`, `cite.bib`, `featured.png/jpg`) |
| Current team | `content/authors/<id>/_index.md` (+ `avatar.jpg`). Order with `weight` (Emily always first) |
| Alumni | `data/alumni.yaml` (name, optional link). Move the person's folder from `content/authors/` to `archive/` |
| Blog posts | `content/blog/` (`.md`, or `.Rmd` rendered by blogdown). Use `summary:` for the card text. `draft: true` hides a post |
| Courses and tutorials | `content/courses/` (tutorial `.html` files are served as-is) |
| Comics, Diversity, Join us | `content/comics/`, `content/diversity/`, `content/prospective/` |
| Menu, email, links | `hugo.toml` |

## Preview locally
`blogdown::serve_site()` needs Hugo 0.139.4 extended: run `blogdown::install_hugo("0.139.4")` once,
and set `options(blogdown.hugo.version = "0.139.4")` in `.Rprofile`. Or run `hugo server` in the site folder.
