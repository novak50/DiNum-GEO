# DiNum-GEO website: notes for Claude

This is the website of the DiNum-GEO research project (Faculty of Civil
Engineering, University of Belgrade, with partners at Durham University and the
British Geological Survey), funded by the Science Fund of the Republic of
Serbia (Dijaspora 2024 programme). The site owner is Novak Joksimović
(`me` in `data/authors/`), who maintains it and talks to you in these sessions.

It is a Hugo site built on the HugoBlox "academic-cv" template and deployed to
GitHub Pages at https://novak50.github.io/DiNum-GEO/ from the `main` branch of
github.com/novak50/DiNum-GEO (see `.github/workflows/deploy.yml`).

## Working rules (from Novak; always follow)

- **Commits are authored by Novak only.** Never add `Co-Authored-By: Claude…`,
  `Claude-Session:` or any other Claude attribution to commit messages or PR
  descriptions, and never commit as Claude or change the git identity/config.
  Only commit when asked.
- Novak often edits files by hand. Read the current file before changing it,
  and never overwrite his edits with an older version.
- Content usually arrives as a Word document in **Serbian**; the site is in
  **English**. Translate faithfully, keep the meaning, fix obvious typos
  (and wrong years), and mention what you changed.
- After a change, build the site and check the result in a browser before
  saying it works (see "Build and preview").

## Build and preview

- Hugo **extended v0.162.0**. Theme code comes from Hugo Modules pinned in
  `go.mod` (`github.com/HugoBlox/kit/modules/blox@v0.0.0-20260527025321-61f41d3667f1`).
- Preview: `hugo server`, then open http://localhost:1313/DiNum-GEO/.
- Production-like build: `hugo --gc --minify` (output in `public/`, ignored by git).
- If a page looks stale, delete `public/` and `resources/` and rebuild.
- The site lives under the **`/DiNum-GEO/` subpath** (`baseURL` in
  `config/_default/hugo.yaml`). A link that works at the root can 404 on the
  live site, so always check links under the subpath.

## Content map

| What | Where | Notes |
|---|---|---|
| Homepage ("About") | `content/_index.md` | `sections:` of blocks: intro `markdown` block + `content-collection` "Recent Activities" (3 newest from `activities/`) |
| News | `content/blog/<slug>/index.md` | list page `content/blog/_index.md` (`view: article-grid`) |
| Activities | `content/activities/<slug>/index.md` | own page, same layout as News; `show_in_news: true` in front matter also lists the post on News (one copy, no duplicate) |
| Publications | `content/papers/<slug>/index.md` | list title "Publications", `view: citation`; nav label "Publications", URL stays `papers/` |
| Team page | `content/team/index.md` | `team-showcase` block (members with `user_groups: [Team]`), partner logo marquee + 3-column partner description grid, funding block |
| People | `data/authors/<slug>.yaml` | `name`, `role`, `bio`, `links`, `user_groups`; photo at `assets/media/authors/<slug>.jpg` |
| Navbar | `config/_default/menus.yaml` | About, Team, News (`/blog`), Activities (`activities/`), Publications (`papers/`), Contact |
| Partner logos | `static/media/partners/` | `grf_logo.png` (Faculty of Civil Eng., Belgrade), `ub_logo.png`, `durham_logo.png`, `bgs_logo.png`; in content use `{{< relimg "media/partners/x.png" "alt" >}}` |

### Team members (`data/authors/`)

| Slug | Person | Role on site |
|---|---|---|
| `me` | Novak Joksimović (site owner, `is_owner: true`) | Team Member |
| `milos` | Miloš Marjanović | Principal Investigator |
| `ksenija` | Ksenija Micić | Team Member |
| `jelena-ninic` | Jelena Ninić (Durham University) | Project Partner |
| `tijana-jovanovic` | Tijana Jovanović (British Geological Survey) | Project Partner |

`vojkan-jovicic`, `zehao-ye` and `hoang-giang-bui` are external co-authors
(minimal profiles, not in `Team`). On paper pages, non-Team authors are shown
as plain, unlinked text on purpose.

## Writing a News or Activities post

Copy the front matter of an existing post (e.g. `content/blog/icsmge/index.md`):

- `title`, `date` (event start date, `YYYY-MM-DD`), `authors`, `categories: [Research]`,
  `tags: [Academic, Research]`, `image: {preview_only: true, caption:}`, `summary:`.
- `authors:` is who posted it; by convention `- me` unless the post is a team
  effort (then e.g. `me`, `ksenija`, `milos`).
- Photos go in the post's own folder. The card thumbnail is a file named
  `featured.*` in that folder (or `cover.image` / `image.filename` in front
  matter); `cover:` gives the big banner on the post page. Posts with several
  photos use the inline HTML carousel copied from `content/blog/acuus/index.md`
  (`dinumgeoCarouselMove`). No photo at all is fine: the card then simply has
  no image area.
- Unknown links from the source document are kept as the literal placeholder
  `More about the publication at the link: ***.` until Novak supplies them.

## Pitfalls we already hit (do not repeat)

1. **Author tags must be written one way per person.** In `authors:` lists use
   the data-file slug for `me`, `milos`, `ksenija`, but the **quoted full name**
   for everyone else (`"Jelena Ninić"`, `"Tijana Jovanović"`, `"Vojkan Jovičić"`,
   `"Zehao Ye"`, `"Hoang-Giang Bui"`), which is how the papers list them. Hugo
   treats `jelena-ninic` and `"Jelena Ninić"` as two different taxonomy terms
   that both publish to `/authors/jelena-ninic/`; one silently overwrites the
   other and the author page randomly loses posts.
2. **Links under the subpath:** use `relURL` / `relimg` with paths that do
   **not** start with `/` (`printf "authors/%s/" $slug | relURL`). A leading
   `/` skips the `/DiNum-GEO/` prefix and 404s on GitHub Pages.
3. **Dark mode is a class, not the OS setting.** The site toggles a `.dark`
   class on `<html>` (moon icon). In custom CSS use `.dark .my-class {…}`,
   never `@media (prefers-color-scheme: dark)`; the media query made the
   partner text white-on-white for visitors whose OS was dark.
4. **Narrow text columns come from Tailwind `prose`/`max-w-prose`** (about 65
   characters). The `markdown` block and `single.html` both cap width this way.
   The partner grid on the Team page escapes it with a full-bleed wrapper
   (`width: 100vw; margin-left/right: calc(50% - 50vw)`).
5. `site.GetPage` for taxonomy terms is keyed by the raw term (`"jelena ninić"`),
   not the URL slug. To check whether an author page exists, compare against
   `path.Base .RelPermalink` of `(site.GetPage "/authors").Pages` (see the
   team-showcase override).
6. Go template comments (`{{/* */}}`) never reach the HTML, so they can't be
   used as markers to check which template file is active.

## Theme overrides in this repo

To change theme behaviour, copy the vendored file to the same path under
`layouts/` and edit it. Find vendored files with `hugo config mounts` or in the
module cache (`…/pkg/mod/github.com/!hugo!blox/kit/modules/blox@…`). Page
blocks live in the module's `blox/<name>/block.html` and are mounted at
`layouts/_partials/hbx/blocks/<name>/block.html`.

| File | Why it exists |
|---|---|
| `layouts/_partials/hbx/blocks/team-showcase/block.html` | Filter by `user_groups`; link a member only if their author page exists; subpath-safe links |
| `layouts/_partials/page_author.html` | Author row on paper pages: Team members as cards, others as plain text, aligned |
| `layouts/_partials/page_author_card.html` | Subpath-safe profile link |
| `layouts/_partials/views/card.html` | No empty grey image box when a post has no image |
| `layouts/_partials/views/article-grid--start.html` | A list with a single post uses one full-width column |
| `layouts/blog/list.html` | News list also includes Activities posts with `show_in_news: true` |
| `layouts/papers/list.html` | Centred "Publications" heading, no intro text |
| `layouts/team/single.html` | Renders the Team page's `sections:` |
| `layouts/_shortcodes/relimg.html` | `<img>` with a subpath-safe `src` for files in `static/` |
| `layouts/_partials/hooks/head-end/github-button.html` | GitHub buttons script |

## Open items

- **About page (homepage) redesign:** Novak will share a reference website (URL
  plus screenshots) whose layout he likes. Rebuild the layout with DiNum-GEO's
  own text, images and colours; don't copy the other site's branding, wording
  or photos, and say up front if an effect (heavy animation, video) isn't
  worth it on this theme.
- The navbar **Contact** link points to `contact/`, but no `content/contact/`
  page exists, so it 404s. Create the page (or remove the menu entry) once
  Novak says what it should contain.
- Optional: widen the text column on post/paper pages (`max-w-none` in a
  site copy of `single.html`). Discussed, not done.
- Upcoming posts listed in the source document: a workshop on 22.12.2026 and an
  academic visit to Durham University (Nov–Jan).
- Replace the `***` publication-link placeholders when Novak sends the links.
- Check `content/blog/kick_off/index.md`: if its `authors:` list uses
  `jelena-ninic` / `tijana-jovanovic`, change them to the quoted full names
  (pitfall 1).
