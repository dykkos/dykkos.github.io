# dykkos.github.io

Personal website: https://dykkos.github.io/

Plain academic index with serif text, a pale paper background, and linked lists.
The homepage has Academic, Project, and Blog sections. Existing PDF URLs are retained.

## AI-safety reading library

`ai-safety.html` links to four category pages in `readings/*.md`.
They include only readings marked read in the TAISI portal in weeks 0–6, captured
2026-11-18: 47 week-level read markers, 46 distinct URLs. Repeated articles retain
both week references. `data/taisi-readings.json` stores the titles, URLs, week references,
and assigned categories. It contains no ratings or private notes. This is a manual snapshot.

The four category Markdown files are the display source; update the JSON inventory
alongside them if revising the selection or categorization.

## Writing a blog note

GitHub Pages uses its built-in Jekyll support to render Markdown into HTML.
No theme or extra plugin is required. The layout is `_layouts/note.html`.

1. Copy `_templates/note.md` into `blog/ai-safety/`, `blog/mathematics/`, or `blog/computer-science/`.
2. Use a name such as `2026-11-18-my-note.md` and set `title`, `note_date`, and
   `blog_category` (exactly `AI Safety`, `Mathematics`, or `Computer Science`).
3. Write Markdown beneath the closing `---`. Set `math: true` for MathJax.
4. Commit to `main`. GitHub Pages renders the note and lists it automatically on
   its category page. The homepage and `blog.html` link to those category pages.

The original two mathematics blog entries now live in `blog/mathematics/*.md`;
old `blog.html#erdos-renyi` and `blog.html#arzela-ascoli` links remain valid.
A plain `python3 -m http.server` previews HTML but does not render Markdown/Liquid;
use Jekyll for a complete local preview, or verify the Pages deployment.

`images/wikiclick-learning-curve.png` is copied unchanged from
`bowen-pixel/WikiClick/figures/learning_curves/LC03_next_link_validation_1000.png`.
It shows offline validation histories, not live-web performance.

## Navigation and illustrations

All pages include footer links to Academic, Project, Experience, Miscellaneous, and GitHub.
`experience.html` lists fellowship and community participation. `misc.html` contains
the captioned SpongeBob and rings-and-ideals illustrations. The displayed name is Bowen Guang.

- `script.html`: Script mini-projects, branch links, and demo pictures (`images/scripts/`).
