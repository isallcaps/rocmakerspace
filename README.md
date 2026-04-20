# ROC Makerspace Documentation

> **Note:** This is an unofficial, community-maintained resource and is not affiliated with or endorsed by Rochester Makerspace organizationally. Rochester Makerspace has its own knowledge management plans in the works — this repo exists in the meantime to make area documentation accessible without waiting on that.

A community documentation repository for area guides, handouts, and reference materials at the [Rochester Makerspace](https://rocmakers.org) — starting with the stained glass area.

The docs live here as Markdown files and are published as a website via [GitHub Pages + Jekyll](https://pages.github.com/). Anyone can read, link to, or contribute — no Google account required.

**→ [View the live docs site](https://isallcaps.github.io/rocmakerspace/)**

---

## Why This Repo Exists

These documents used to live in a personal Google Drive. That worked fine until it didn't — sharing links broke, access was tied to one person's account, and there was no easy way for others to suggest corrections. Moving to a public GitHub repo means:

- Documents are accessible to anyone, permanently
- Changes are tracked and reversible
- Other area leads can use or adapt this structure for their own area's docs
- No single person is the bottleneck

Rochester Makerspace is working toward a more official wiki or knowledge base — when that exists, content here can migrate there. Until then, this fills the gap.

---

## What's Here

Right now the content is focused on the **stained glass area**, but the structure is designed to be reused by any area of the makerspace.

```
stained-glass/        # Stained glass studio guides and handouts
...                   # Future areas can live here as their own folders
_config.yml           # Jekyll configuration for the docs site
```

---

## Viewing the Docs

The rendered site is published at **[https://isallcaps.github.io/rocmakerspace/](https://isallcaps.github.io/rocmakerspace/)**.

If you just want to read the content without navigating the repo, go there.

---

## Running the Site Locally

If you want to preview changes before pushing:

**Prerequisites:** Ruby and Bundler — see the [Jekyll installation guide](https://jekyllrb.com/docs/installation/).

```bash
# Clone the repo
git clone https://github.com/isallcaps/rocmakerspace.git
cd rocmakerspace

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve
```

Then open `http://localhost:4000` in your browser.

---

## Contributing

Found a typo? Have a technique to add? Contributions are welcome.

### Easiest way — edit directly on GitHub

1. Navigate to the file you want to edit
2. Click the pencil ✏️ icon (top right of the file view)
3. Make your changes and describe them in the commit message
4. Submit a pull request

### For bigger changes

1. Create a branch: `git checkout -b your-branch-name`
2. Edit or add Markdown files in your area's folder
3. Push and open a pull request

Pull requests are reviewed and tested locally before merging — so don't worry about breaking anything, just submit and we'll sort it out together.

**Writing guidelines:**
- Files are standard Markdown (`.md`)
- Each file should start with Jekyll front matter (see any existing file for the pattern)
- Keep language practical and accessible — these are handouts for people new to a tool or material

---

## Adding a New Area

If you're an area lead and want to use this structure for your own documentation:

1. Create a new folder in the root of the repo with your area's name (e.g., `laser-cutter/`)
2. Add your Markdown files there
3. Update `_config.yml` if you need a new nav section (or open an issue and ask)
4. Submit a pull request — it'll be tested locally and merged

No need to maintain a separate fork; everything can live here together.

---

## Structure of a Doc File

All content files follow this pattern:

```markdown
---
layout: default
title: Your Page Title
parent: Area Name
nav_order: 1
---

# Your Page Title

Content here...
```

The front matter (the `---` block) tells Jekyll how to build the navigation and page layout.

---

## Tech Stack

| Thing | What it does |
|---|---|
| Markdown | All content is written in `.md` files |
| [Jekyll](https://jekyllrb.com/) | Converts Markdown to a static website |
| [Just the Docs](https://just-the-docs.github.io/just-the-docs/) | Jekyll theme — clean docs layout with sidebar nav |
| [GitHub Pages](https://pages.github.com/) | Hosts the built site for free |

---

## License

Content in this repository is shared for community use. See [LICENSE](LICENSE) for details.

---

*Unofficial community resource maintained by stained glass area volunteers. Not affiliated with or endorsed by Rochester Makerspace organizationally. Questions? Open an issue or find us at the space.*
