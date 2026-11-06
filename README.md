# Shourie37.github.io

Personal site of Shourie Amireddy. It is a static site for GitHub Pages: plain HTML and CSS, with no build step, no JavaScript, and no external requests.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | All page content. |
| `style.css` | All styles. Light and dark colors follow the system setting. |
| `404.html` | Page that GitHub Pages shows for an unknown path. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

## Edit the content

- Each section in `index.html` is a `<section>` with an `id` (`about`, `work`, `projects`, `skills`, `education`, `contact`). The nav links point to these ids. If you add a section, add a nav link too.
- Each project card sits between two comments, for example `<!-- PROJECT: raft-kv START -->` and `<!-- PROJECT: raft-kv END -->`. To change a card, edit the block. To move a card, move the whole block.
- A card has a name with a link, a one-line description, a `Result:` line, and tags.
- Cards under "Building now" have no result yet. When a project is ready, move its block to "More projects", add a `Result:` line and a tag list, and remove the `card-wip` class and the `status` line.
- Take every fact and number from the profile README or the project README. Do not add claims that have no source.
- Colors are CSS variables at the top of `style.css`. The dark theme is in the `prefers-color-scheme: dark` block.

## Preview locally

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open http://127.0.0.1:8000/.

## Publish

Push to the `main` branch of the `Shourie37.github.io` repository. In the repository settings, set Pages to deploy from `main` at the root.
