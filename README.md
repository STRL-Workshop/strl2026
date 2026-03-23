# STRL 2026 Website

Website for the **5th International Workshop on Spatio-Temporal Reasoning and Learning (STRL 2026)**, co-located with [IJCAI-ECAI 2026](https://ijcai-26.org/) in Bremen, Germany.

Built with [Hugo](https://gohugo.io/).

## Local Development

1. [Install Hugo](https://gohugo.io/installation/) (extended edition recommended).
2. Clone this repository and navigate to the `website/` directory:
   ```bash
   cd website
   ```
3. Start the development server:
   ```bash
   hugo server -D
   ```
4. Open [http://localhost:1313/strl2026/](http://localhost:1313/strl2026/) in your browser.

## Updating Content

- **Important dates, topics, schedule**: Edit the YAML files in `data/`.
- **Organizers, advisory committee, PC**: Edit the corresponding YAML files in `data/`.
- **Prose sections** (introduction, submission guidelines): Edit `content/_index.md`.
- **Site-wide settings** (title, venue, contact email): Edit `hugo.toml`.

## Building for Production

```bash
hugo --minify
```

The generated site will be in the `public/` directory.

## Deployment

The site is automatically deployed to GitHub Pages via the GitHub Actions workflow in `.github/workflows/hugo.yml` on every push to `main`.

The site is hosted at: https://strl-workshop.github.io/strl2026/
