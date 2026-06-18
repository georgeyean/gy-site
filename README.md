# George Yean — Academic Website

Hugo-based academic website for George Yean, PhD Candidate in Government at Harvard University.

**Live site:** https://georgeyean.github.io/gy-site/

## Quick start (local preview)

```bash
brew install hugo          # one-time setup
cd gy-site
hugo server
```
Then open http://localhost:1313/gy-site/

## Editing your site

See [UPDATING.md](UPDATING.md) for step-by-step instructions with no local setup required.

## Structure

| Path | What it controls |
|------|-----------------|
| `hugo.yaml` | Name, email, social links, photo, CV path |
| `content/_index.md` | Bio paragraphs, awards, news items |
| `data/papers.yaml` | All papers (working, published, JMP) |
| `data/teaching.yaml` | Teaching history |
| `data/projects.yaml` | Software / R packages |
| `static/images/` | Headshot (`photo.jpg`) |
| `static/files/` | PDFs (CV, papers) |
| `static/css/style.css` | All visual styling |
